---
permalink: /
---
# MindWork AI

MindWork AI is the GitHub organization behind [AI Studio](https://github.com/MindWorkAI/AI-Studio). In addition to AI Studio, we offer other repositories, such as [ERI](https://github.com/MindWorkAI/ERI), the "(E)xternal (R)etrieval (I)nterface" for AI Studio and other LLM tools.


## AI Studio

[AI Studio](https://github.com/MindWorkAI/AI-Studio) is a desktop app for daily work with LLMs. The app is available for macOS, Windows, and Linux, and can be used for free (including for commercial work). However, we appreciate donations.

![MindWork AI Studio - Home](media/AI%20Studio%20Home.png)
![MindWork AI Studio - Assistants](media/AI%20Studio%20Assistants.png)


## ERI - (E)xternal (R)etrieval (I)nterface

The [ERI](https://github.com/MindWorkAI/ERI) is the External Retrieval Interface for [AI Studio](https://github.com/MindWorkAI/AI-Studio) and other tools. The ERI acts as a contract between decentralized data sources and, e.g., AI Studio. The ERI is implemented by the data sources, allowing them to be integrated into AI Studio later. This means that the data sources assume the server role and AI Studio (or any other LLM tool) assumes the client role of the API. This approach serves to realize a [Retrieval-Augmented Generation](https://en.wikipedia.org/wiki/Retrieval-augmented_generation) (RAG) process with external data. You can imagine it like this: Hypothetically, when Wikipedia implemented the ERI, it would vectorize all pages using an [embedding method](https://en.wikipedia.org/wiki/Word_embedding). All of Wikipedia's data would remain with Wikipedia, including the [vector database](https://en.wikipedia.org/wiki/Vector_database) (decentralized approach). Then, any AI Studio user could add Wikipedia as a data source to significantly reduce the hallucination of the LLM in knowledge questions.

When you want to integrate your own local data into AI Studio, you don't need an ERI. Instead, AI Studio will offer an RAG process for this in the future. Is your organization interested in integrating internal company data into AI Studio? [Here](swagger-ui.html) you will find the [interactive documentation](swagger-ui.html) of the related OpenAPI interface.

Links:
- [ERI repository with example implementation in .NET / C#](https://github.com/MindWorkAI/ERI)
- [Interactive documentation aka Swagger UI](swagger-ui.html)
- [ERI specification](v1.0-production.json), which you could use with tools like [OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator).
