# 🌟 LLM Hallucination Index - RAG Special 🌟

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/352971390-316d4cdd-f8d4-4bbd-ad6f-e8949e3b1854.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQxOTUsIm5iZiI6MTcyMjI1Mzg5NSwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTcxMzkwLTMxNmQ0Y2RkLWY4ZDQtNGJiZC1hZDZmLWU4OTQ5ZTNiMTg1NC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTUxMzVaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00MjZiYWNiNWMyYmQ1MDJhZjEwMDIwMmIzNzhkNjhmNzhhYzIxMGRmYmUzZTQyOTNhODU5N2Q2OTU2MDNmZDMxJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.oHKDbYUJIMAtiDZ6oUzIufx4ei1ENGqtoNM_fvwcXLA" />
</p>

<p align="center">
  <a href="https://www.rungalileo.io/hallucinationindex">https://www.rungalileo.io/hallucinationindex</a>
</p>

# About the Index

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/352972431-6c0a60b4-2574-4cfe-9e5a-00469f5484d7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQxOTUsIm5iZiI6MTcyMjI1Mzg5NSwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTcyNDMxLTZjMGE2MGI0LTI1NzQtNGNmZS05ZTVhLTAwNDY5ZjU0ODRkNy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTUxMzVaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yMzNjNmYzZGI5NmYyNjc0MGVkZmJlZTg1ODc0ZDNkM2VjNWE3ZmFiZjliNjFmMTEyMzYwMmU4NWVkNDUwOTU2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.b0ABK4mYQCALXkOkmTfuFOBrUyTr4RdhFUVK4x65s8E" />
</p>

# Attributes Tested

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

![image](https://private-user-images.githubusercontent.com/138050654/352951799-3e3a55e1-f36e-4767-9ad7-778b6f7c6a56.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQxOTUsIm5iZiI6MTcyMjI1Mzg5NSwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTUxNzk5LTNlM2E1NWUxLWYzNmUtNDc2Ny05YWQ3LTc3OGI2ZjdjNmE1Ni5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTUxMzVaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mY2YzOTU1NGQ0MmM0ODkzZTI2MTllMzVhNDczNDMzZDYwNmMyOThhNjk1M2FjMDM2NWJmZWFlMjc1ODRmNDVlJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.5z4p0e7YhmM6S4zBnz3N5hu1_Tf09_VNcuBJ88ppYIo)

# Major Trends

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/352950366-9d145cc9-7ad1-4995-b8c3-0f87c7ceb7c4.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTUwMzY2LTlkMTQ1Y2M5LTdhZDEtNDk5NS1iOGMzLTBmODdjN2NlYjdjNC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wMzExZWM2MDdiZTc0NTIzYjdkN2I2ZWVjYjJiZjNmZjRhMmRkOGVjOTdkOTM2MGRhMjUzMzQ3OTIxYzM0MzYzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.7HqNTIu6exw86NnfNoNki8M2lMMCze963bn3z_LJN3E" style="max-width: 200%; width: 800px;" />
</p>

# Overall Winners

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/352952355-2f43e64e-5ddf-46d7-8710-867802891b98.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTUyMzU1LTJmNDNlNjRlLTVkZGYtNDZkNy04NzEwLTg2NzgwMjg5MWI5OC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02ZDgzZTE3NmQ1Yjc1ZDRkNzEzMTQyZTA4ZTFiNzYxNDhhYmEyNjgyMGRjOWYyMzBkMGM5YjU1ZjFiNWVhOGM0JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.U1YVcy3q8EWFIVDardxj7NQ4fmjK7hykjBScZZCDoQM" />
</p>

# Short Context RAG Insights

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/352952848-c336f509-4c31-46d4-bd2e-c3635a729783.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTUyODQ4LWMzMzZmNTA5LTRjMzEtNDZkNC1iZDJlLWMzNjM1YTcyOTc4My5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wYzkzYTBjMjAxMWM1ZDRhYjkxZmMzMmE3YjlhYjg0OWI1YTIyNjhiOWUyY2Q3NDMyNWM4ZGMyYzY4NDRjZDQyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.BP3tUbMv6LWpYmRlJ46LVj4vhYUNj6EHD4mZp-pUH5Q" />
</p>

# Medium Context RAG Insights

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/352954140-78bd024f-b4ad-4f81-a88b-b5d8e9450cc2.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTU0MTQwLTc4YmQwMjRmLWI0YWQtNGY4MS1hODhiLWI1ZDhlOTQ1MGNjMi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1jNTBiOWFlMmI2ZjNiN2ZlNmIyNzMxYzRmNzRmOWVkZjVhNDU5ZWRlMGE0NzMwZTI5OTlkMDIzZDg0NWEwMWE2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.qi7gZxtnqiPGlCONcmW82DZOp01AT9CJPoXz2VMqpaQ" />
</p>

# Long Context RAG Insights

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/352954466-11babd08-c407-46de-acdf-9cc7926cf3df.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUyOTU0NDY2LTExYmFiZDA4LWM0MDctNDZkZS1hY2RmLTljYzc5MjZjZjNkZi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03NGJlOTcxZTVhMjQzZDg3NWRjNTllOTU5ZGY2YWQzNDA2ZmMwOGU2YTBhMDYyY2E4ZTc4MzEyNmU1ZTQzNjU3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.urKgxxlF5WUFsvjjok00dsNir-72Pgwb_tDWcN0kBAw" />
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

### Evaluation

Adherence to context was evaluated using a custom LLM-based assessment, checking for the relevant answer within the response.

# Hallucination Detection

To evaluate a model’s propensity to hallucinate, we employed a high-performance evaluation technique to assess contextual adherence and factual accuracy. Learn more about Galileo’s [Context Adherence](https://www.rungalileo.io/research) and [ChainPoll](https://www.rungalileo.io/blog/chainpoll).

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/353020342-97e9f9df-cf74-4f45-9889-416b7f78d9b5.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUzMDIwMzQyLTk3ZTlmOWRmLWNmNzQtNGY0NS05ODg5LTQxNmI3Zjc4ZDliNS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hZTZlMjEzYjA3OWU2NmNlYzhjNzVmNGQwZDAxNjhkYWUyMDg5ZWY0ODQwNzE0NjBmMzcyYzZjOWRiNTkxZjk3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.5JNjz_bl0Pv92fX-kY-IQtDqpLM5_7mnNv-cP7szFYg" />
</p>

# Inner Working of ChainPoll

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/353020580-001280a4-89eb-44f8-958b-370b96bb32c9.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUzMDIwNTgwLTAwMTI4MGE0LTg5ZWItNDRmOC05NThiLTM3MGI5NmJiMzJjOS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03YzIwZjQ5MjVkMWVkZmJlZWE4NzhiNWEyNjY2MTAzOTc1MDk5NTY2ZTk2NTAwMmU0MDk1OGUxMjZhZDlhYzhiJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.MRgmW1UtTLYWRMZe1rfbeMA3UIOjXmktUe-xpbufqPA" />
</p>

# About Galileo

<p align="center">
  <img src="https://private-user-images.githubusercontent.com/138050654/353028249-c0e037da-e48b-46f9-bbb6-c438825f8537.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjIyNTQ1NzQsIm5iZiI6MTcyMjI1NDI3NCwicGF0aCI6Ii8xMzgwNTA2NTQvMzUzMDI4MjQ5LWMwZTAzN2RhLWU0OGItNDZmOS1iYmI2LWM0Mzg4MjVmODUzNy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcyOVQxMTU3NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0xZTQ5MDU3NmM4YjUzOGM0YmFhYjcxMjNhNjlhNWRkOGM3ZmM1ZWY3OThjNDdlMjA3MjQyMWNkNTZjMTc0YTNjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.U8Cg2NHyJ1E24RTgRgG_1olfQD41qYeGP0E5PwfAvWo" />
</p>

# Get the Full Report with More Insights 🌟

For an in-depth understanding, we recommend checking out [https://www.rungalileo.io/hallucinationindex](https://www.rungalileo.io/hallucinationindex).
