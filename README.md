# Sustainable AI

The past 50 years has seen a dramatic increase in the amount of computing capability per person, in particular, those enabled by AI. Despite the positive societal benefits, AI technologies can come with significant environmental implications. To scale AI sustainably, we need to make AI and computing more broadly efficient and flexible. Going beyond efficiency, we look into designing and optimizing AI models and computing infrastructures across the lifecycle. This repository provides resources from our research innovations and artifacts to talks and education materials to sustainably advance towards artificial general intelligence.

## Overview: Scaling AI Sustainably
The past 50 years has seen a dramatic increase in the amount of computing capability per person. Since the introduction of the first commercially available microprocessor -- the Intel 4004 released in 1971 – the number of transistors in a computer die has increased by over a million fold. Accelerating knowledge discovery in science and engineering demands even higher computation capability beyond what a single microprocessor can offer. 

High-performance computing infrastructures, from supercomputers solving weather forecasting, molecular modeling, and other complex computational problems to AI training clusters, connect tens of thousands of processors using advanced networking gears to further scale up computation capability. For example, the Frontier supercomputer -- the world’s first exascale supercomputer -- comes with more than 37,000 Graphics Processing Units (GPUs) to deliver more than 1 quintillion calculations per second. And, to propel our reach to artificial general intelligence, AI superclusters, such as Google’s Tensor Processing Unit (TPU) based AI Hypercomputer or Meta’s Research SuperCluster (RSC), also rely on horizontal scaling to achieve high performance, scalability, and efficiency. 

With data centers of domain-specific hardware specialization, the computing industry has achieved many orders-of-magnitude efficiency improvements through decades of technological innovations. Such efficiency improvement is key to keep the energy use of data centers globally constant. Between 2010 and 2018, the compute instances in global data centers increased by 5.5 times while the overall energy use increased by merely 0.06 times [1].    

AI is revolutionizing the entire industry, from education and medicine to e-commerce, finance, and entertainment. OpenCatalyst uses AI to discover new electrocatalysis for efficient renewable energy storage. AlphaFold uses AI to predict protein structures rapidly that has the potential to revolutionize the entire biological science domain. FarmBeats uses AI to improve farming efficiency. AI is changing the way we live, learn, communicate, and interact with each other in a profound manner. Despite the positive societal benefits, the development of AI technologies necessitates an increase in data center energy use and associated greenhouse gas emissions, from the rising demand of computing resources. Between 2019 and 2021, the amount of data used for AI model training increased by more than two times, corresponding to a more than 20 times model size increase [2]. In fact, since the inception of AlexNet in 2012, the number of parameters of the state-of-the-art AI models have been increasing exponentially into the scale of trillions of parameters and requiring terabytes of memory capacity for storage. The AI scaling trend is pushing the frontier of computing infrastructures. 

The first step is to understand AI’s carbon impact across its lifecycle holistically. AI’s lifecycle carbon impact comes from use of AI systems, called operational carbon footprint, as well as from manufacturing of AI systems and data center construction materials, called embodied carbon footprint. 

### Operational Carbon Footprint 
Operational carbon footprint is defined as the carbon emissions (defined as carbon dioxide equivalent (CO2e)) associated with the electricity consumed. For a key production recommendation model, the energy consumption breakdown is roughly 30:30:40 over the key phases of Data, Experimentation / Training, and Inference. For example, the operational carbon footprint of llama3 model training is estimated to produce 2,290 tonnes of carbon emissions using the GPU Thermal Design Power (TDP) of 700W and the average emission factor of the US grids. In reality, AI workflows typically involve dozens, if not hundreds, of training runs to produce a final model. Once a model is trained to meet the desirable accuracy level, it is further optimized to serve various product use cases. In case of the language translation model, the inference footprint can double the training carbon footprint over its entire model lifetime.

### Embodied Carbon Footprint 
AI’s carbon impact goes beyond emissions associated with the electricity needed to power the models (operational energy use) to include the embodied emissions of the required infrastructure, such as, semiconductor manufacturing, and steel and cement used for data center construction. AI systems used for model training and inference at scale come with manufacturing carbon emissions that are produced during the production of system hardware. Carbon embodied in AI system hardware constitutes a substantial portion to AI’s overall carbon footprint. Taking the multilingual translation task as an example, the model’s overall lifecycle carbon footprint is approximately four times higher than the operational carbon footprint of model training. 
 
For consumer electronics, embodied carbon footprint is a more significant than operational carbon footprint over the computing device’s lifecycle, with a rough breakdown of 80 to 20 [3]. As consumer electronics evolve into wearables that germinate the next wave of computing, additional demand in data centers will be required to support the new computing paradigm. And, we expect a similar embodied to operational carbon footprint breakdown for wearables, such as smart glasses. Tomorrow, we will have augmented reality with contextual AI capability. This is an important time for us, computer system designers, to innovate with sustainability in mind. What do sustainability-first design principles look like for the next wave of computing? 

## Carbon Tools

### CarbonNaaS 
To enable carbon-guided AI model-hardware design space exploration, we design CarbonNaaS 

![Sustainable AI Landing Page 1](https://github.com/user-attachments/assets/914f4231-9ec8-4c6b-9386-efa3f5e5412b)

### ACT
https://github.com/facebookresearch/ACT

To enable carbon-guided computer system design, we design ACT --- an architectural carbon modeling tool --- to enable sustainable computer system design. ACT comprises an analytical, architectural carbon footprint model and use-case dependent optimization metrics to estimate the carbon footprint of hardware --- embodied carbon. ACT estimates greenhouse gas (GHG) emissions from hardware manufacturing based on workload characteristics, hardware specifications, semiconductor fab characteristics, and environmental factors.

ACT addresses a crucial gap in quantifying and enabling sustainability-driven hardware design space exploration for sustainability to be considered as a first-order design objective, alongside performance, power, and area.

![Sustainable AI Landing Page 2](https://github.com/user-attachments/assets/7f5d5314-4770-4c5a-9bf7-dd7b0b95c783)

### Carbon Explorer

To enable carbon-guided datacenter computing, we design Carbon Explorer --- 

![Sustainable AI Landing Page 3](https://github.com/user-attachments/assets/e6462066-0758-47c1-8f88-379b2e697f3e)
