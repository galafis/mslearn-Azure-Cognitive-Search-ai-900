<div align="center">

# ☁️ Azure Cognitive Search — AI Search para Indexação e Consulta de Dados

**[Português](#português) | [English](#english)**

[![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)](https://azure.microsoft.com/)
[![AI Search](https://img.shields.io/badge/Azure_AI_Search-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)](https://azure.microsoft.com/products/ai-services/cognitive-search)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

*Projeto prático do bootcamp Microsoft Azure AI Fundamentals (DIO) — indexação cognitiva e consulta semântica de avaliações de clientes / Hands-on project from the Microsoft Azure AI Fundamentals bootcamp (DIO) — cognitive indexing and semantic querying of customer reviews*

</div>

---

## Português

### 📋 Sobre o Projeto

Laboratório prático que demonstra o uso do **Azure AI Search** para indexar e consultar dados enriquecidos com habilidades de IA. O cenário simula uma rede de cafeterias que precisa analisar avaliações de clientes para entender sentimentos, extrair frases-chave e gerar insights acionáveis.

### 🏗️ Arquitetura

```mermaid
graph TD
    A[📄 Documentos<br/>Reviews .docx] -->|Upload| B[Azure Blob Storage<br/>coffee-reviews]
    B -->|Indexação| C[Azure AI Search<br/>coffee-index]
    D[Azure AI Services<br/>Cognitive Skills] -->|Enriquecimento| C
    C -->|Projeções| E[Knowledge Store<br/>Tabelas + Imagens]
    C -->|Consulta| F[Search Explorer<br/>Filtros + Sentimento]

    style A fill:#e1f5fe
    style B fill:#fff3e0
    style C fill:#e8f5e9
    style D fill:#f3e5f5
    style E fill:#fce4ec
    style F fill:#e0f2f1
```

### 🔧 Recursos Criados

| Recurso | Finalidade |
|---------|-----------|
| Azure AI Search | Gerenciamento de indexação e consulta |
| Azure AI Services | Habilidades cognitivas (sentimento, frases-chave, OCR) |
| Storage Account | Armazenamento de documentos brutos (Blob containers) |
| Knowledge Store | Dados enriquecidos persistidos (tabelas + projeções) |

### 📸 Etapas Documentadas

1. **Criação do Azure AI Search** — configuração do serviço de pesquisa
   ![Azure AI Search](prints/criação%20de%20resourse,%20criação%20de%20azure%20ai%20search,%20configuração%20e%20deploy.jpeg)

2. **Azure AI Services** — recurso LAB4-AI-900 para enriquecimento cognitivo
   ![Azure AI Services](prints/criação%20do%20lab%20e%20services.jpeg)

3. **Storage Account** — contêiner de blob para documentos
   ![Storage Account](prints/criação%20store%20account.jpeg)

4. **Contêiner coffee-reviews** — importação e indexação dos dados
   ![Coffee Reviews](prints/coffe-reviews%20criado.jpeg)

5. **Search Explorer** — filtragem por sentimento (negativo/positivo)
   ![Search Explorer](prints/search%20explorer%20por%20sentimentos.jpeg)

6. **Knowledge Store** — dados enriquecidos extraídos pelas habilidades de IA
   ![Knowledge Store](prints/dados%20enriquecidos%20extraídos%20pelas%20habilidades%20de%20IA.jpeg)

7. **Projeções de imagem** — imagens armazenadas dos documentos
   ![Imagem armazenada](prints/imagem%20armazenada%20do%20documento..jpeg)

8. **Tabelas de entidades** — frases-chave capturadas pelo Knowledge Store
   ![Tabelas](prints/Há%20uma%20tabela%20para%20cada%20entidade%20no%20índice.jpeg)

### 💡 Insights e Aplicabilidade

- **Análise de sentimento** permite identificar insatisfação de clientes em tempo real
- **Extração de frases-chave** automatiza a categorização de feedback
- **Filtros semânticos** possibilitam consultas refinadas por localização, produto e sentimento
- Aplicável em: varejo, hospitalidade, e-commerce, saúde, educação

### 📚 Referências

- [Azure AI Search Documentation](https://learn.microsoft.com/azure/search/)
- [Bootcamp DIO — Microsoft Azure AI Fundamentals](https://www.dio.me/)

---

## English

### 📋 About the Project

Hands-on lab demonstrating **Azure AI Search** for indexing and querying data enriched with AI skills. The scenario simulates a coffee shop chain that needs to analyze customer reviews to understand sentiment, extract key phrases, and generate actionable insights.

### 🏗️ Architecture

```mermaid
graph TD
    A[📄 Documents<br/>Reviews .docx] -->|Upload| B[Azure Blob Storage<br/>coffee-reviews]
    B -->|Indexing| C[Azure AI Search<br/>coffee-index]
    D[Azure AI Services<br/>Cognitive Skills] -->|Enrichment| C
    C -->|Projections| E[Knowledge Store<br/>Tables + Images]
    C -->|Query| F[Search Explorer<br/>Filters + Sentiment]

    style A fill:#e1f5fe
    style B fill:#fff3e0
    style C fill:#e8f5e9
    style D fill:#f3e5f5
    style E fill:#fce4ec
    style F fill:#e0f2f1
```

### 🔧 Resources Created

| Resource | Purpose |
|----------|---------|
| Azure AI Search | Indexing and query management |
| Azure AI Services | Cognitive skills (sentiment, key phrases, OCR) |
| Storage Account | Raw document storage (Blob containers) |
| Knowledge Store | Persisted enriched data (tables + projections) |

### 📸 Documented Steps

1. **Azure AI Search creation** — search service configuration
2. **Azure AI Services** — LAB4-AI-900 resource for cognitive enrichment
3. **Storage Account** — blob container for documents
4. **coffee-reviews container** — data import and indexing
5. **Search Explorer** — sentiment filtering (negative/positive)
6. **Knowledge Store** — AI-enriched data extraction
7. **Image projections** — stored document images
8. **Entity tables** — key phrases captured by Knowledge Store

### 💡 Insights and Applicability

- **Sentiment analysis** enables real-time customer dissatisfaction detection
- **Key phrase extraction** automates feedback categorization
- **Semantic filters** allow refined queries by location, product, and sentiment
- Applicable in: retail, hospitality, e-commerce, healthcare, education

### 📚 References

- [Azure AI Search Documentation](https://learn.microsoft.com/azure/search/)
- [DIO Bootcamp — Microsoft Azure AI Fundamentals](https://www.dio.me/)

---

## 👤 Autor / Author

**Gabriel Demetrios Lafis**

[![GitHub](https://img.shields.io/badge/GitHub-galafis-181717?style=flat&logo=github)](https://github.com/galafis)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-gabriel--lafis-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/gabriel-lafis/)

## 📄 Licença / License

Este projeto está licenciado sob a Licença MIT — veja o arquivo [LICENSE](LICENSE) para detalhes.

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
