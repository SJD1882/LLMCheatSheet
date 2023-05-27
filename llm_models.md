# **LLM: Non-Exhaustive List of Models**

<p align="center">
  <img src="images/stochastic_predictors.PNG" alt="Image Description" width="750px">
</p>

## Proprietary LLMs

| Name | Chatbot | Model<br>Creator | Parameters<br>(billions) | Release Date |
| -- | -- | -- | -- | -- |
| [GPT-3](https://www.semanticscholar.org/paper/Language-Models-are-Few-Shot-Learners-Brown-Mann/6b85b63579a916f705a8e10a49bd8d849d91b1fc) | ChatGPT | OpenAI,<br>Microsoft | 175 | (LLM) May 2020<br>(Chatbot) Oct. 2022 |
| GPT-3.5 Turbo | ChatGPT Premium | OpenAI,<br>Microsoft | < 175 | April 2023
| [GPT-4](https://www.semanticscholar.org/paper/GPT-4-Technical-Report-OpenAI/8ca62fdf4c276ea3052dc96dcfd8ee96ca425a48) | ChatGPT Premium<br>Bing AI | OpenAI<br>Microsoft | ??? | April 2023
| [LaMDA](https://www.semanticscholar.org/paper/LaMDA%3A-Language-Models-for-Dialog-Applications-Thoppilan-Freitas/b3848d32f7294ec708627897833c4097eb4d8778) | Bard | Google | 137 | (LLM) Jan. 2022<br>(Chatbot) Fev. 2023
| Gopher | N/A | Deepmind<br>Google | 280 | N/A |
| Chinchilla | N/A | Deepmind<br>Google | 70 | N/A |
| PaLM 1 | N/A | Google | 540 | N/A |
| [PaLM 2](https://www.semanticscholar.org/paper/PaLM-2-Technical-Report-Anil-Dai/eccee350691708972370b7a12c2a78ad3bddd159) | Bard | Google | [340](https://www.cnbc.com/2023/05/16/googles-palm-2-uses-nearly-five-times-more-text-data-than-predecessor.html)* | May 2023 |
| [Claude](https://www.anthropic.com/index/introducing-claude) | Poe | Anthropic | ??? | March 2023 |

*Source: CNBC

## Consumer LLMs, finetuned variants and alignment datasets

### **LLMs**

It is important to distinguish the open sourced LLM from the variant that was finetuned (RLHF) on a specific dataset of instructions (RLHF-Supervised Fine-Tuning) and/or a dataset of LLM output preferences (RLHF-Proximal Policy Optimization).

| Name | Model<br>Creator | Parameters<br>(billions) | Release Date | Licence |
| -- | -- | -- | -- | -- |
| [Flan-T5-XL<br>Flan-T5-XXL](https://www.semanticscholar.org/paper/Scaling-Instruction-Finetuned-Language-Models-Chung-Hou/5484d228bfc50efbac6e86677bc2ec2ee4ede1a6) | Google | 3<br>11 | Oct. 2022 | Open source
| [LLaMA](https://www.semanticscholar.org/paper/LLaMA%3A-Open-and-Efficient-Foundation-Language-Touvron-Lavril/57e849d0de13ed5f91d086936296721d4ff75a75) | Meta | 7<br>13<br>30<br>65 | Fev. 2023 | Non-commercial
| [Pythia](https://www.eleuther.ai/papers-blog/pythia-a-suite-for-analyzing-large-language-modelsacross-training-and-scaling) | EleutherAI | 3<br>7<br>12 | April 2023 | Open source |
| [StabilityLM](https://github.com/Stability-AI/StableLM) | StabilityAI | 3<br>7<br>15 (TBD)<br>30 (TBD)<br>65 (TBD)<br>175 (TBD) | April 2023 | Open source |
| [MPT](https://www.mosaicml.com/blog/mpt-7b) | MosaicML | 7 | May 2023 | Open source |
| [Starcoder](https://huggingface.co/blog/starcoder)<br>(mainly for code<br>generation) | HuggingFace | 15 | May 2023 | OpenRAIL<br>(open source<br>with use-case<br>restrictions)
| [OpenLLaMA](https://github.com/openlm-research/open_llama) | Berkeley AI Research<br>| TBD | TBD | Open source |

### **Alignment finetuned Variants of Consumer LLMs**

I will mostly be checking out the finetuned GPTQ and GGML LLMs from HuggingFace user [TheBloke](https://huggingface.co/TheBloke) and other official providers (e.g. LMSYS, Databricks, OpenAssistant). I will be listening new models each time I was successful in running them on Google Colab.

| Name | Model<br> Creator | Model<br>Finetuner | Parameters<br>(billions) | Fintuned<br>Release | Licence | RLHF-SFT<br>Dataset | RLHF-PPO<br>Dataset | GPU |
| -- | -- | -- | -- | -- | -- | -- | -- | -- |
| [Fastchat-T5](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0)| Google | LMSYS | 3 | April 2023 | Non-commercial<br>(dataset) | ShareGPT<br>(70k chats) | No | T4 15Go |
| [Pythia 3B (Dolly)](https://huggingface.co/databricks/dolly-v2-3b) |  EleutherAI | Databricks | 3 | April 2023 | Open source | Databricks Dolly<br>(15k instructs) | No | T4 15Go |
| [Pythia 7B (Dolly)](https://huggingface.co/databricks/dolly-v2-7b) | EleutherAI | Databricks | 7 | April 2023 | Open source | Databricks Dolly<br>(15k instructs) | No | T4 15Go |
| [LLaMA 13B (GPT4 x Vicuna) (Unrestricted)](https://huggingface.co/TheBloke/gpt4-x-vicuna-13B-GPTQ) | Meta | NousResearch | 13 | April 2023 | Non-commercial (model, dataset) | ShareGPT 35K Unrestricted  | No | T4 15Go
| [LLaMA 13B (WizardLM x Vicuna)](https://huggingface.co/TheBloke/wizard-vicuna-13B-GPTQ) | Meta | Microsoft China | 13 | April 2023 | Non-commercial (model, dataset) | Wizard EvolInstruct 70k | No | T4 15Go
| [LLaMA 13B (WizardLM) (Unrestricted)](https://huggingface.co/TheBloke/Wizard-Vicuna-13B-Uncensored-GPTQ) | Meta | Microsoft China | 13 | April 2023 | Non-commercial (model, dataset) | WizardLM EvolInstruct Uncensored 50k | No | T4 15Go |


### **Alignment finetuning datasets**

- **Alpaca Finetuning Datasets**
    - [Stanford Alpaca SelfInstruct 52K](https://huggingface.co/datasets/tatsu-lab/alpaca)
        - *Non-commercial*
        - For less than 600$ and 3 hours of finetuning on 8 80GB A100s, researchers from Stanford University generated a dataset of 52K instructions with OpenAI's "Text-davicini-003" (GPT-3) following the SelfInstruct ([Wang et al., 2022](https://www.semanticscholar.org/paper/Self-Instruct%3A-Aligning-Language-Model-with-Self-Wang-Kordi/bbe93c90b7b87939cd064c805858feca61a3234d)), then finetuned on those instructions.
    - [Microsoft Alpaca GPT-4 52K](https://huggingface.co/datasets/c-s-ale/alpaca-gpt4-data)
        - *Non-commercial*
        - Follows Stanford's Alpaca methodology but used here GPT-4 for generating the 52k instructions ([Peng et al., 2023](https://www.semanticscholar.org/paper/Instruction-Tuning-with-GPT-4-Peng-Li/9e8cb8c91a0acb6e661b58ad724aa758490f2bea))
- **Databricks Dolly**
    - [Databricks Dolly 15K](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
        - *Open source*
        - Dataset of over 15K instructions generated by Databricks' employees following the InstructGPT methodology. The dataset contains instructions covering "brainstorming, classification, closed QA, generation, information extraction, open QA, and summarization".
- **ShareGPT**
    - [ShareGPT](https://sharegpt.com/)
        - *Non-commercial*
        - Users upload their prompts/replies from ChatGPT (any version), which can then be used for cheaply finetuning LLMs without relying on human annotators. The legality of using ShareGPT is rather murky but it seems that simply using it for research purposes, back office applications (not exposing to clients) or even commercial use might not be restricted as long as the LLM finetuned on ShareGPT doesn't compete with OpenAI's ChatGPT (not unlike the controversy where Google was accused of finetuning their chatbot Bard on GPT outputs).
    - [ShareGPT Unrestricted 35K](https://huggingface.co/datasets/anon8231489123/ShareGPT_Vicuna_unfiltered)
        - *Non-commercial*
- **WizardLM Evol-Instruct**
    - [WizardLM EvolInstruct 70K](https://huggingface.co/datasets/ehartford/WizardLM_alpaca_evol_instruct_70k_unfiltered)
        - *Non-commercial*
        - 70k instructions that followed WizardLM's EvolInstruct methodology. It starts with the normal Alpaca approach for generating a dataset of instructions but then the authors ask GPT-4 to rewrite the initial instructions into more complex ones. The idea is that with more complex and especially diverse instructions, this will improve the performance of LLMs with relatively low parameter count (7B, 13B), which seems to be the case since WizardLM 7B is as of May 2023 seen as the top 7B open source LLM.
    - [WizardLM EvolInstruct Unrestricted 50K](https://huggingface.co/datasets/ehartford/WizardLM_alpaca_evol_instruct_70k_unfiltered)
        - *Non-commercial*
        - The original EvolInstruct 70k filtered of OpenAI's alignment contraints ("I'm sorry...", "As an AI language model, I cannot..."), reduced down to the 50K complex instructions (following WizardLM's EvolInstruct methodology). The LLaMA 7B trained on this unrestricted dataset produces better performances than the restricted vanilla LLM, which might indicate that there is an "alignment tax" (excessive moral alignment decreases model capacity to respond to user queries).
