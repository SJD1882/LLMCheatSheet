# **LLM: Research Papers**

As Large Language Models (LLM) have exploded in popularity since the unveiling of ChatGPT by OpenAI in October 2022, research and commercial interest over LLMs has led to a tsunami of research contributions. This is an attempt to curate the list of research articles, with a description of the main findings of each paper to the best of my knowledge. This list is non-exhaustive.

## Summaries

- [Zhao, Wayne Xin et al. “**A Survey of Large Language Models**.” ArXiv abs/2303.18223 (April 2023)](https://www.semanticscholar.org/paper/A-Survey-of-Large-Language-Models-Zhao-Zhou/1d29334cfbe9a1a943082058876f0c22d44c62fd)
    - Great place to start. Setups a rigourous taxonomy for what constitutes an LLM. For the authors, an NLP text generation transformer can be reasonably classified as an LLM when it has over 10 billion parameters (for reference BERT only has 300 million parameters, LLaMA biggest model has 65 billion and GPT-3 has 175 billion). 
- [Bowman, Sam. “**Eight Things to Know about Large Language Models**.” ArXiv abs/2304.00612 (April 2023)](https://www.semanticscholar.org/paper/Eight-Things-to-Know-about-Large-Language-Models-Bowman/23a183676b28269e7a427c41da7329b6326a9f17)
    - In one of the 8 points presented by Bowman, the "emergent abilities" claim from Wei et al. [2022] (that on previously "unsolvable" tasks once a certain large threshold of parameter count is reached, LLM unexpectedly performance jumps massively) is scrutinized. The author finds that of the 202 tasks evaluated by Wei et al., only 33% of them are truly "emergent", i.e. see discontinuous jumps in performance.

- [Yang, Jingfeng et al. “**Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond**.” ArXiv abs/2304.13712 (April 2023)](https://www.semanticscholar.org/paper/Harnessing-the-Power-of-LLMs-in-Practice%3A-A-Survey-Yang-Jin/131c6f328c11706de2c43cd16e0b7c5d5e610b6a)
    - Main takeaway of this paper is that while LLMs outperform previous state-of-the-art  transformers (BERT, RoBERTa, BART) on tasks that require out-of-sample generalization, on domain-specific tasks previous supervised methods still outperform LLMs (e.g. English-Kazakh translation).

## Foundational LLMs

- [Brown, Tom B. et al. “**Language Models are Few-Shot Learners**.” ArXiv abs/2005.14165 (2020)](https://www.semanticscholar.org/paper/Language-Models-are-Few-Shot-Learners-Brown-Mann/6b85b63579a916f705a8e10a49bd8d849d91b1fc)
    - **GPT-3** (175B parameters) by OpenAI which powers chatbot ChatGPT (free-tier version). Proprietary LLM.

- [Thoppilan, Romal et al. “**LaMDA: Language Models for Dialog Applications**.” ArXiv abs/2201.08239 (2022): n. pag.](https://www.semanticscholar.org/paper/LaMDA%3A-Language-Models-for-Dialog-Applications-Thoppilan-Freitas/b3848d32f7294ec708627897833c4097eb4d8778)
    - **LaMDA** (137B parameters) by Google which powered chatbot Bard (to be replaced soon by PaLM 2). Proprietary LLM.

- [Touvron, Hugo et al. “**LLaMA: Open and Efficient Foundation Language Models**.” ArXiv abs/2302.13971 (2023)](https://www.semanticscholar.org/paper/LLaMA%3A-Open-and-Efficient-Foundation-Language-Touvron-Lavril/57e849d0de13ed5f91d086936296721d4ff75a75)
    - **LLaMA** (7B to 65B parameter variants) by Meta. Released to the public under a non-commercial licence. Now ubiquitous among the research and AI enthusiast community, seeing countless finetuned variants (e.g. Alpaca, Vicuna, Open Assistant, WizardLM, Manticore, etc.).

- [OpenAI. “**GPT-4 Technical Report**.” ArXiv abs/2303.08774 (2023)]()
    - **GPT-4** (unknown parameter count) by OpenAI which powers chatbot ChatGPT and can be used with external plugins (premium version). Proprietary LLM.

- [Biderman, Stella Rose et al. “**Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling**.” ArXiv abs/2304.01373 (2023)](https://www.semanticscholar.org/paper/Pythia%3A-A-Suite-for-Analyzing-Large-Language-Models-Biderman-Schoelkopf/64e20f2abc15d5cf04a682df5a1265bd45ba9fe7)
    - **Pythia** (3B, 7B, 12B) by EleutherAI (ex-OpenAI veterans). Open source with free commercial licence.

- [Anil, Rohan et al. “**PaLM 2 Technical Report**.” (2023).](https://www.semanticscholar.org/paper/PaLM-2-Technical-Report-Anil-Dai/eccee350691708972370b7a12c2a78ad3bddd159)
    - **PaLM 2** (340B parameters) by Google which is expected to replace LaMDA as the LLM powering chatbot Bard. Proprietary LLM.
    - The 340B figure was first reported by CNBC on May 16th 2023 ([Source](https://www.cnbc.com/2023/05/16/googles-palm-2-uses-nearly-five-times-more-text-data-than-predecessor.html))

## Alignment Fine-Tuning Methods (RLHF)

## Theoretical Considerations on LLMs

## Quantization of LLMs

## Alignment and Ethics (Empirical Issues)

## Alignment and Ethics (alternatives to RLHF)

## Economics

## Philosophy