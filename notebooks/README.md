# **Large Language Models Resources Repository - Colab Notebooks**

Some ideas of implementations or use-cases with open source LLMs:

### **Basics**

- **Running HuggingFace vanilla variants of open source LLMs with Langchain** 
  - [ ] Pythia-Dolly 12B supervised finetuned on Databricks Dolly 15k instruction dataset
- **Running GPTQ variants of open source LLMs with HuggingFace and Langchain**
  - [x] [LLaMA-WizardVicuna 13B supervised finetuned on Vicuna and WizardLM instruction datasets](GPTQ_LLaMA_WizardLM_13B.ipynb)
  - [ ] LLaMA-WizardLM 33B supervised finetuned on WizardLM instruction datasets
  - [ ] LLaMA-Guacano 33B supervised finetuned on 9k sampled OpenAssistant Conversations dataset
  - [ ] LLaMA-RLHF-OASST1 33B RLHF-finetuned on OpenAssistant Conversations dataset
- **Running GGML variants (llama.cpp compatible) of open source LLMs with Langchain**
  - [x] [LLaMA-WizardVicuna 13B supervised finetuned on Vicuna and WizardLM instruction datasets](GGML_LLaMA_WizardLM_13B.ipynb)
  - [ ] LLaMA-Guacano 65B supervised finetuned on 9k sampled OpenAssistant Conversations dataset

### **Defensive frameworks**

- [ ] Using Anthropic's Constitutional AI to better moderate the outputs of unrestricted LLMs

### **Applications**

- [ ] Use case: Using Open Source LLMs with Langchain for Web Search (e.g. Wikipedia, DuckDuckGo)
- [ ] Use case: Using Open Source LLMs with Langchain for reading multiple PDF files
- [ ] Use case: Using Open Source LLMs with Langchain for story writing

### **AGI**
- [ ] Reproducing ChaosGPT with an open source LLM and BabyAGI
