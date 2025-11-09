# DSC180A - Methodology Assignment 4

**Name:** Leah Seseri 

**Email:** lseseri@ucsd.edu

**Section:** B08

**Mentor:** Aaron Boussina and Karandeep Singh

### **What is the most interesting topic covered in your domain this quarter?**
The most interesting topic covered in my domain is information retrieval in the medical domain using LLMs especially in challenging contexts like unstructured health records. Factors like documentation length, negation, or acronyms make it difficult to use simple LLMs to retrieve relevant medical information efficiently. Exploring different ideas like combining a keyword search, using hybrid RAG, or using agentic RAG to solve the complications of information retrieval in the medical field, makes this topic highly interesting and beneficial for the future of LLMs in the medical field. Also, exploring test-time scaling to improve the performance of LLMs by increasing computational resources without retraining is another angle that is exciting in the field of information retrieval. 

### **Describe a potential investigation you would like to pursue for your Quarter 2 Project.**
A potential investigation I would like to pursue for my quarter two project is to benchmark different retrieval approaches in health records for medical events. I would like to define a set of target medical events like sepsis and then implement multiple different retrieval strategies such as traditional RAG or agentic RAG. I would evaluate performance on multiple things not just F1 or accuracy, but also computational cost, inference calls, and the carbon footprint. As mentioned earlier, test-time scaling would be beneficial to investigate by running multiple inference passes to improve retrieval performance without retraining the LLM. This investigation could produce a robust benchmarking framework for medical information retrieval which is currently lacking standardized evaluations. 

### **What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**
A potential change I would make to the approach taken in my current quarter one project would be to more formally define what my ground truth is in the retrieval pipeline. Currently I have evaluated ground truth on small curated datasets or MedQA questions which is not generalizable or reliable because real world clinical notes are large, unstructured, and unpredictable. I would like to implement a needle in a haystack approach with real or generated medical notes that are embedded in patient charts and then validate these ground truths with human review or synthetic augmentation. To determine what approach is more efficient, I would compare my retrieval strategies across both real and synthetic setups which would provide a more systematic benchmark and reduce the reliance on limited datasets. 

### **What other techniques would you be interested in using in your project?** 
Some additional techniques I would be interested in using in my project would be exploring LLM based majority voting and Monte Carlo sampling techniques to improve retrieval reliability. Majority voting is a way to improve reliability by asking the same questions and selecting the answer that occurs most frequently which helps reduce variance in the model’s output. Similarly, Monte Carlo sampling repeatedly focuses the model to observe the distribution of possible responses, allowing an estimation of confidence or uncertainty in the retrieval decisions. Another technique would be implementing energy aware benchmarking to measure the computation cost and carbon emissions for the different retrieval strategies.