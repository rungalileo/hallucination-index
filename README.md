# 🌟 LLM Hallucination Index - RAG Special🌟

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/316d4cdd-f8d4-4bbd-ad6f-e8949e3b1854" />
</p>

<p align="center">
  <a href="https://www.rungalileo.io/hallucinationindex">https://www.rungalileo.io/hallucinationindex</a>
</p>

# About the Index

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/6c0a60b4-2574-4cfe-9e5a-00469f5484d7" />
</p>

# Attributes  Tested

There were two key LLM attributes we wanted to test as part of this Index - context length and open vs. closed-source.

## Context Length

With the rising popularity of RAG, we wanted to see how context length affects model performance. Providing an LLM with context data is akin to giving a student a cheat sheet for an open-book exam. We tested three scenarios:

| Context Length | Task Description |
| -------------- | ----------- |
| Short Context  | Provide the LLM with < 5k tokens of context data, equivalent to a few pages of information. |
| Medium Context | Provide the LLM with 5k - 25k tokens of context data, equivalent to a book chapter. |
| Long Context   | Provide the LLM with 40k - 100k tokens of context data, equivalent to an entire book. |

## Open vs. Closed Source

The open-source vs. closed-source software debate has waged on since the Free Software Movement (FSM) in the late 1980s. This debate has reached a fever pitch during the LLM Arms Race. The assumption is closed-source LLMs, with their access to proprietary training data, will perform better, but we wanted to put this assumption to the test.

## Prompting Techniques

We experimented with a prompting technique known as Chain-of-Note, which has shown promise for enhancing performance in short-context scenarios, to see if it similarly benefits medium and long contexts.

# Models Evaluated

We tested 22 models, 10 closed-source models and 12 open-source models, from leading foundation model brands like OpenAI, Anthropic, Meta, Google, Mistral, and more.

![image](https://gist.github.com/user-attachments/assets/3e3a55e1-f36e-4767-9ad7-778b6f7c6a56)

# Major Trends

   <p align="center">
     <a href="https://gist.github.com/user-attachments/assets/9d145cc9-7ad1-4995-b8c3-0f87c7ceb7c4">
       <img src="https://gist.github.com/user-attachments/assets/9d145cc9-7ad1-4995-b8c3-0f87c7ceb7c4" alt="Image Description" style="max-width: 200%; width: 700px;" />
     </a>
   </p>

# Overall Winners

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/2f43e64e-5ddf-46d7-8710-867802891b98" />
</p>

# Short Context RAG Insights

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/c336f509-4c31-46d4-bd2e-c3635a729783" />
</p>

# Medium Context RAG Insights

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/78bd024f-b4ad-4f81-a88b-b5d8e9450cc2" />
</p>

# Long Context RAG Insights

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/11babd08-c407-46de-acdf-9cc7926cf3df" />
</p>

# Methodology

## Short Context RAG (SCR)

We evaluated SCR using a rigorous set of datasets to test the model's robustness in handling short contexts. One of our key methodologies was Chainpoll with GPT-4o. This involves polling the model multiple times using a chain of thought technique, allowing us to:

1. Quantify potential hallucinations.
2. Offer context-based explanations, a crucial feature for RAG systems.

## Medium and Long Context RAG (MCR & LCR)

Our focus here was on assessing models’ ability to comprehensively understand extensive texts in medium and long contexts. The procedure involved:

- Extracting text from 10,000 recent documents of a company.
- Dividing the text into chunks and designating one as the "needle chunk."
- Constructing retrieval questions answerable using the needle chunk embedded in the context.

### Context Lengths Evaluated

- **Medium**: 5k, 10k, 15k, 20k, 25k tokens
- **Long**: 40k, 60k, 80k, 100k tokens

### Task Design Considerations

1. All text in context must be from a single domain.
2. Responses should be correct even with short context, confirming the influence of longer contexts.
3. Questions should not be answerable from pre-training memory or general knowledge.
4. Measure the influence of information position by keeping everything constant except the location of the needle.
5. Avoid standard datasets to prevent test leakage.

### Effect of Prompting Technique on Performance

We experimented with a prompting technique known as Chain-of-Note, which has shown promise for enhancing performance in short-context scenarios, to see if it similarly benefits medium and long contexts.

## Evaluation

Adherence to context was evaluated using a custom LLM-based assessment, checking for the relevant answer within the response.

# Hallucination Detection

To evaluate a model’s propensity to hallucinate, we employed a high-performance evaluation technique to assess contextual adherence and factual accuracy. Learn more about Galileo’s [Context Adherence](https://www.rungalileo.io/research) and [ChainPoll](https://www.rungalileo.io/blog/chainpoll).

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/97e9f9df-cf74-4f45-9889-416b7f78d9b5" />
</p>

# Inner Working of ChainPoll

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/001280a4-89eb-44f8-958b-370b96bb32c9" />
</p>

# About Galileo

<p align="center">
  <img src="https://gist.github.com/user-attachments/assets/c0e037da-e48b-46f9-bbb6-c438825f8537" />
</p>

# Get the Full Report with More Insights 🌟

For an in-depth understanding, we recommend checking out [https://www.rungalileo.io/hallucinationindex](https://www.rungalileo.io/hallucinationindex).
