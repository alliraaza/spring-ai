# Spring AI Projects

A collection of hands-on **Spring AI projects and proof-of-concepts** exploring Generative AI, RAG, local LLMs, vector databases, MCP, and AI application development using Java and Spring Boot.

The repository is structured as a collection of independent projects, with each project focusing on a specific Spring AI capability or architecture pattern.

## 🚀 Technology Stack

* **Java**
* **Spring Boot**
* **Spring AI**
* **Spring Framework**
* **Maven**
* **Ollama**
* **Large Language Models (LLMs)**
* **Retrieval-Augmented Generation (RAG)**
* **PostgreSQL / pgvector**
* **Model Context Protocol (MCP)**
* **REST APIs**
* **Docker** / **Podman**

## 📂 Projects

| Project     | Description                                             |
| ----------- | ------------------------------------------------------- |
| `ai-rag-mem` | RAG application using Spring AI and InMemory Vector Store  |
| `ai-rag-pg` | RAG application using Spring AI and PostgreSQL/pgvector |
| `ai-ollama` | Local LLM integration using Spring AI and Ollama        |
| `ai-tools-mcp`| Expose tools via Model Context Protocol and Spring AI. `ai-rag-pg` application using MCP cliet to invoke tools   |


> The list above will evolve as new AI projects are added to this repository.

## 🧠 Areas Covered

### Generative AI

Exploring how Java applications can interact with Large Language Models through Spring AI.

Topics include:

* Chat models
* Prompt engineering
* Structured output
* LLM integration
* Local LLM inference
* Model configuration

### Retrieval-Augmented Generation (RAG)

Building applications that combine enterprise documents/data with LLMs to provide context-aware responses.

Typical RAG flow:

```text
Documents
    │
    ▼
Document Loader
    │
    ▼
Text Splitting
    │
    ▼
Embeddings
    │
    ▼
Vector Store
    │
    ▼
Similarity Search
    │
    ▼
Relevant Context
    │
    ▼
LLM
    │
    ▼
Generated Answer
```

The repository includes experiments with both **PostgreSQL/pgvector** and **Qdrant** as vector stores.

### Local AI

Using **Ollama** to run LLMs locally without depending entirely on cloud-based AI APIs.

Example architecture:

```text
Spring Boot Application
        │
        ▼
     Spring AI
        │
        ▼
      Ollama
        │
        ▼
      Local LLM
```

### Model Context Protocol (MCP)

Exploring MCP-based integration between AI applications and external tools/services.

MCP enables an AI application to interact with tools and data sources through a standardized protocol.

```text
        AI Application
              │
              ▼
         Spring AI
              │
              ▼
             MCP
              │
       ┌──────┼──────┐
       ▼      ▼      ▼
     Tool   Tool   Resource
```

## 🏗️ Repository Structure

```text
spring-ai/
│
├── ai-rag-mem/
│   ├── src/
│   ├── pom.xml
│   └── README.md
│
├── ai-rag-pg/
│   ├── src/
│   ├── pom.xml
│   └── README.md
│
├── ai-ollama/
│   ├── src/
│   ├── pom.xml
│   └── README.md
│
├── ai-tools-mcp/
│   ├── src/
│   ├── pom.xml
│   └── README.md
│
└── README.md
```

Each project is maintained as an independent Maven/Spring Boot application and contains its own README with setup and usage instructions.

## ⚙️ Prerequisites

Depending on the project, you may need:

* JDK 21+
* Maven 3.9+
* Docker/Podman
* PostgreSQL/pgvector
* Ollama

Check the individual project README for the exact requirements.

## 🏃 Running a Project

Navigate to the project directory:

```bash
cd ai-rag-pg
```

Build the application:

```bash
mvn clean package
```

Run it:

```bash
mvn spring-boot:run
```

Individual projects may require additional infrastructure such as PostgreSQL, Qdrant, or Ollama.

## 🗄️ Infrastructure

Some projects use locally hosted infrastructure.

### PostgreSQL / pgvector

Used for storing application data and vector embeddings for RAG applications.

```text
Spring AI
    │
    ▼
PostgreSQL
    │
    └── pgvector
```

### Ollama

Ollama provides local LLM inference.

```text
Spring AI → Ollama → Local LLM
```

## 🎯 Purpose

The purpose of this repository is to build practical experience with **enterprise-grade Generative AI application development using Java and Spring**.

The projects focus on understanding how AI capabilities can be integrated into traditional enterprise application architectures rather than treating AI as a standalone technology.

Key objectives include:

* Understand Spring AI fundamentals
* Build production-oriented RAG pipelines
* Integrate local and cloud LLMs
* Work with vector databases
* Experiment with MCP
* Explore AI tool calling
* Evaluate different LLMs and embedding models
* Understand AI application architecture
* Apply Generative AI patterns to enterprise applications

## 🔬 POC / Learning Repository

This repository is primarily a **technical exploration and POC repository**.

Projects may evolve as technologies, Spring AI APIs, models, and architectural approaches change.

Individual projects may therefore use different:

* LLMs
* Embedding models
* Vector databases
* Spring AI features
* Infrastructure configurations

## 📚 Learning Areas

The repository serves as a practical reference for:

```text
Spring AI
   │
   ├── Chat Models
   ├── Prompt Engineering
   ├── Embeddings
   ├── Vector Stores
   ├── RAG
   ├── Tool Calling
   ├── MCP
   ├── Structured Output
   └── Local LLMs
          │
          ├── Ollama
          └── Open-source Models
```

## 📌 Status

🚧 **Active Development**

New Spring AI experiments and POCs will continue to be added to this repository.

## 👤 Author

**Ali Raza**

Senior Application Architect / Tech Lead

Focus areas:

* Java & Spring
* Microservices
* Event-Driven Architecture
* Cloud-Native Applications
* Generative AI
* RAG
* Enterprise AI Architecture

---

⭐ This repository is a practical exploration of building **AI-powered applications with Java and Spring AI**.

