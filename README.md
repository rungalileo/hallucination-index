# 🌟 LLM Hallucination Index 🌟
## About the Index 💥
The Hallucination Index is an ongoing initiative to evaluate and rank the most popular LLMs based on propensity to hallucinate. The index uses a comprehensive set of datasets, chosen for their diversity and ability to challenge the model’s abilities to stay on task. 

**Why**: There has yet to be an LLM benchmark report that provides a comprehensive measurement of LLM hallucinations. After all, measuring hallucinations is difficult, as LLM performance varies by task type, dataset, context and more. Further, there isn’t a consistent set of metrics for measuring hallucinations. 

**What**: The Hallucination Index ranks popular LLMs based on their propensity to hallucinate across three common task types - question & answer without RAG, question and answer with RAG, and long-form text generation. 

**How**: The Index ranks leading 11 LLMs performance across three task types. The LLMs were evaluated using 7 popular datasets. To measure hallucinations, the Hallucination Index employs 2 metrics, Correctness and Context Adherence, which are built with the state-of-the-art evaluation method Chainpoll.

We share full details about our methodology [here](http://rungalileo.io/hallucinationindex).

## LLM Rankings for Q&A with RAG
Task: A model that, when presented with a question, uses retrieved information from a given dataset, database, or set of documents to provide an accurate answer. This approach is akin to looking up information in a reference book or searching a database before responding.

![LLM Rankings for QA with RAG](https://user-images.githubusercontent.com/138050654/283152708-7ef81e54-7b40-4f4d-b416-90c414f877bd.png)

## LLM Rankings for Q&A without RAG
Task: A model that, when presented with a question, relies on the internal knowledge and understanding that the AI model has already acquired during its training. It generates answers based on patterns, facts, and relationships it has learned without referencing external sources of information.

![LLM Rankings for QA without RAG](https://user-images.githubusercontent.com/138050654/283152214-e30b0b6c-1fa2-4484-88b2-5a554903bc93.png)

## LLM Rankings for Long-Form Text Generation
Task: Using generative AI to create extensive and coherent pieces of text such as reports, articles, essays, or stories. For this use-case, AI models are trained on large datasets to understand context, maintain subject relevance, and mimic a natural writing style over longer passages.

![LLM ranking for long form text generation](https://user-images.githubusercontent.com/138050654/283153011-e4cb1107-7e61-4032-879c-3644819482d5.png)

Note: Rankings were last updated on November 15, 2023.

## Evaluation metrics ✨
The metrics used to evaluate output quality and propensity for hallucination are powered by [ChainPoll](https://arxiv.org/abs/2310.18344).


ChainPoll, developed by Galileo Labs, is an innovative and cost-effective hallucination detection method for large language models (LLMs), and RealHall is a set of challenging, real-world benchmark datasets. Our extensive comparisons show ChainPoll's superior performance in detecting LLM hallucinations, outperforming existing metrics such as with a significant margin in accuracy, transparency, and efficiency, while also introducing new metrics for evaluating LLMs' adherence and correctness in complex reasoning tasks.

Learn more about our experiment and results over [here](http://rungalileo.io/hallucinationindex).

![chainpoll metrics](https://user-images.githubusercontent.com/138050654/283151959-48d35b24-4bd3-4f2e-97b1-7ee811fa070e.png)

## Models evaluated

**Open AI**
- GPT-4-0613
- GPT-3.5-turbo-1106
- GPT-3.5-turbo-0613
- GPT-3.5-turbo-instruct

**Meta**
- Llama-2-70b-chat
- Llama-2-13b-chat
- Llama-2-7b-chat

**Hugging Face**
- Zephyr-7b-beta

**Mosaic**
- MPT-7b-instruct

**Mistral**
- Mistral-7b-instruct-v0.1

**TII UAE**
- Falcon-40b-instruct

## What next?
We are excited about this initiative and plan to update Hallucination Index on a quarterly basis. To get an LLM added to the Hallucination Index reach out [here](https://www.rungalileo.io/hallucinationindex).