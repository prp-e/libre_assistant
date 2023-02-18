# Model Studies

## List of Models

- [BLOOM](https://huggingface.co/bigscience/bloom)
- [BLOOMZ](https://huggingface.co/bigscience/bloomz)
- [OPT-175B](https://opt.alpa.ai/)
- [Jurassic](https://ai21.com)
- Others

## Introduction

In order to have a generic generative chatbot like _ChatGPT_ what we need is a language model. Language models are usually trained on a certain language and they do their job pretty well on that particular language, so in order to get a good result we also may need to fine-tune that model. In this documet, some of famous models such as BLOOM, BLOOMZ and OPT are reviewed and their pros and cons are listed. In this document, we simply check the functionality of the model and _how easy it is to fine-tune them_. 

### Why not GPT-3?

The simple reason is that it's more expensive than expected. The other reason is it's not an _open source model_ so even if we use the _fine-tune API_ we still can't claim that the model is free, libre or open-source. 

The final reason is that there are quiet a few open-source __UI__'s for GPT-3 available, so this is meaningless to create one more.

### Why not creating a language model?

It's simple. Creating an LLM (_Large Language Model_) costs millions of dollars and one of my goals is to keep everything as economical as possible.

## Model Studies

### BLOOM

| Pros | Cons |
|:----------------:|:----------------:|
| available in 1B, 1.3B, 7B and 176B | Nothing between 7B and 176B |
| Great on English text generation   | Sucks at generating in other languages |
| Great on code completion           | Sucks at instructional commands        |
| Easy to access on HuggingFace      | Hard to deploy locally                 |
|                                    | Hard to fine-tune                      |
|                                    | Poor sampling (hallucinations & repetitions) |

### BLOOMZ

Everything about _BLOOM_ is also honest about BLOOMZ with one exception. It's really great on instructions. But we still have to deal with over explanations, hallucinations and unnecessary repetitions in the answers.

### OPT-175B

| Pros | Cons |
|:----------------:|:----------------:|
| Has more weights from 125m to 175B | |
| | No guide line of fine-tuning has been released |
| | No coherent results in many cases |
| | Hard to deploy the large model    |
| Good at conversations | |
| Good at taking instructions | |
| | No repeats but hallucinates _a lot_ |
