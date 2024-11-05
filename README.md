---
permalink: /
---
# MindWork AI

MindWork AI is the GitHub organization behind [AI Studio](https://github.com/MindWorkAI/AI-Studio). In addition to AI Studio, we offer other repositories, such as [EDI](https://github.com/MindWorkAI/EDI), the "(E)xternal (D)ata AP(I)" for AI Studio.


## AI Studio

[AI Studio](https://github.com/MindWorkAI/AI-Studio) is a desktop app for daily work with LLMs. The app is available for macOS, Windows, and Linux, and can be used for free (including for commercial work). However, we appreciate donations.


## EDI - (E)xternal (D)ata AP(I)

THe [EDI](https://github.com/MindWorkAI/EDI) is the External Data API for [AI Studio](https://github.com/MindWorkAI/AI-Studio). The EDI acts as a contract between decentralized data sources and AI Studio. The EDI is implemented by the data sources, allowing them to be integrated into AI Studio later. This means that the data sources assume the server role and AI Studio assumes the client role of the API. This approach serves to realize a Retrieval-Augmented Generation (RAG) process with external data. You can imagine it like this: Hypothetically, when the Wikipedia implemented the EDI, it would vectorize all pages using an [embedding method](https://en.wikipedia.org/wiki/Word_embedding). All of Wikipedia's data would remain with Wikipedia, including the [vector database](https://en.wikipedia.org/wiki/Vector_database) (decentralized approach). Then, any AI Studio user could add Wikipedia as a data source to significantly reduce the hallucination of the LLM in knowledge questions.

When you want to integrate your own local data into AI Studio, you don't need an EDI. Instead, AI Studio will offer an RAG process for this in the future. Is your organization interested in integrating internal company data into AI Studio? [Here](swagger-ui.html) you will find the [interactive documentation](swagger-ui.html) of the related OpenAPI interface.