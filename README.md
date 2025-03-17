# Enhancing Metadata Enrichment for Efficient Enterprise Technical Knowledge Retrieval using LLMs and RAG

A research project demonstrating the transformative impact of metadata enrichment in retrieval-augmented generation (RAG) systems for improving information retrieval accuracy and response quality in large, unstructured documentation.

![Architecturee](https://raw.githubusercontent.com/PranavMishra17/MetadataEnrichment-for-RAG/refs/heads/main/arch.png)

[Project Poster](https://github.com/PranavMishra17/MetadataEnrichment-for-RAG/blob/main/Final_Poster.pdf)

## Project Overview

This project introduces a framework for metadata enrichment using large language models (LLMs) to improve accessibility and contextual relevance in enterprise documentation systems. The research focuses on AWS S3 documentation as a test case, developing and evaluating three distinct retrieval approaches:

1. **Content-only Retriever**: Uses standard document chunks without enhancement
2. **Combined Retriever**: Employs weighted retrieval (70% content, 30% metadata)
3. **Elastic Retriever**: Enhanced retrieval with reranking model applied to the combined method

![Tools and software](https://raw.githubusercontent.com/PranavMishra17/MetadataEnrichment-for-RAG/refs/heads/main/image_2025-03-17_135848454.png?token=GHSAT0AAAAAAC6BV6HJOA25HYBQ3JVXRR6MZ6YOJSQ)

## Methodology

The project uses a systematic pipeline with key stages:

- **Document Processing**: Converting unstructured data (PDFs) to processable format
- **Metadata Enrichment**: Applying techniques like summarization, keyword extraction with RAKE and KeyBERT, semantic relationship mapping, and hierarchical structure annotation
- **Embedding Generation**: Creating vector embeddings for efficient retrieval
- **Vector Database Integration**: Storage of vectors alongside generated metadata
- **Retrieval Response Generation**: Using LLMs to interpret queries and generate responses

## Key Results

The research demonstrates several important findings:

- **Content+Metadata** approach achieved the highest faithfulness (0.8691) and lowest hallucination (0.1309)
- **Elastic*** excelled in precision (0.9859), NDCG (0.9874), and coverage (0.7460)
- **Combined** approach achieved the best balance of accuracy and efficiency
- Optimal retrieval performance was observed at K=5, balancing precision and computational efficiency

## Components

- **Backend Processing**: Built on LangChain and Pinecone for data pipelines and embeddings
- **Semantic Chunking**: Divides data into meaningful, context-preserving segments
- **Prompt Engineering**: Uses sophisticated prompts with initial system instructions for improved accuracy
- **Evaluation Framework**: Comprehensive metrics for both retrieval effectiveness and response quality

## Evaluation Metrics

The system was evaluated using both:

1. **Retrieval Performance Metrics**:
   - Precision/Recall
   - Mean Reciprocal Rank (MRR)
   - Normalized Discounted Cumulative Gain (NDCG)
  
![Retriever Eval]((https://raw.githubusercontent.com/PranavMishra17/MetadataEnrichment-for-RAG/refs/heads/main/image_2025-03-17_135919328.png?token=GHSAT0AAAAAAC6BV6HITQMZHCMFO5Q5HPJOZ6YOKHQ))


2. **Response Quality Evaluation**:
   - Faithfulness
   - Coverage
   - Hallucination Rate

![Response Quality Eval](https://raw.githubusercontent.com/PranavMishra17/MetadataEnrichment-for-RAG/refs/heads/main/image_2025-03-17_135949824.png?token=GHSAT0AAAAAAC6BV6HJO6CQ3VDK7V46SLHSZ6YOK6Q)

## Authors

This project was developed by a team at the University of Illinois Chicago, Liautaud Graduate School of Business:
- Pranav Mishra | [Linkedin](https://www.linkedin.com/in/pranavgamedev/)
- Kranti Prakash Yeole | [Linkedin](https://www.linkedin.com/in/krantiyeole/)
- Ramyashree Keshavamurthy | [Linkedin](https://www.linkedin.com/in/ramyashree-keshavamurthy/)
- Professor Fatemeh Sarayloo (advisor)


## Acknowledgments

The Department of Information and Decision Sciences at the University of Illinois at Chicago provided support for this research.
