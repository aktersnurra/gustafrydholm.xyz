---
title: "Retrieval Augmented Generation"
date: 2024-04-26 00:36
tags:
  [
    "deep learning",
    "retrieval augmented generation",
    "vector database",
    "ollama",
    "llm",
  ]
draft: false
---

I implemented a retrieval augmented generation (RAG)
[program](https://github.com/aktersnurra/rag) for fun with the goal of being able to
search my personal library. My focus was to make this run locally with only open
source models. This was achieved with [`ollama`](ollama.com) and
[`sentence-transformers`](https://github.com/UKPLab/sentence-transformers) for
downloading and running these models locally.

However, the project was expanded to
integrate with cohere and their rerank and command-r+ models, since I was curious about
the command-r+ performance. These models can be downloaded and run locally, but it took
ages for my computer to generate any output, since the command-r+ is 104B parameter
model. The obvious and cool benefit of the command-r+ is that it generates citations
from the context in the answer.

Here is a [presentation](/rag.html) that gives a brief overview of what a RAG system
is, and how it can be improved with reranking.
