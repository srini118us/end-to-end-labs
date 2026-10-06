# Enterprise End to End AI Labs

Complete business solutions that combine an application layer, enterprise data, an AI foundation, agents and orchestration, integration, and a human decision point. Each project below lives in its own repository or folder. This repository is the index.

Individual technology labs are in [SAP AI Journey](https://github.com/srini118us/sap-ai-journey). Platform work is in the Databricks, Vertex AI, and Datasphere repositories.

## The pattern

```mermaid
flowchart LR
    A[Business process] --> B[SAP application]
    B --> C[Enterprise data]
    C --> D[AI and ML foundation]
    D --> E[Agents, RAG, MCP]
    E --> F[API and UI]
    F --> G[Human approval]
```

## Projects

| Project | What it does | Stack | Code |
|---|---|---|---|
| Quote to Order Agent | Salesforce opportunity to SAP S/4HANA sales order across clouds, with human approval and read back verification | Vertex AI, LangGraph, Cloud Run, S/4HANA, GenAI Hub | [quote-to-order-agent](https://github.com/srini118us/quote-to-order-agent) |
| Procurement Risk Intelligence | One XGBoost model on SAP AI Core serving four paths: a Joule agent, batch scoring into Datasphere and SAC, governed SBPA approval, and a BDC custom data product consumed by a separate domain | Joule, AI Core, Datasphere, SAC, SBPA, BDC | [uc4-procurement-agent](https://github.com/srini118us/sap-ai-journey/tree/master/joule-joule-studio/uc4-procurement-agent) |
| Governed Multi Agent Finance Insights | BDC Delta Shares consumed in Databricks with a LangGraph supervisor, trust layer, and MLflow tracing | SAP BDC, Databricks, LangGraph, MLflow | [sap-databricks-trial](https://github.com/srini118us/databricks-journey/tree/main/sap-databricks-trial) |
| Cashflow Forecasting Agent | Conversational forecasts with per company models and plain language explanations | Joule, AI Core, AutoTS, SHAP, MCP | [cashflow-forecast](https://github.com/srini118us/sap-ai-journey/tree/master/ai-core/cashflow-forecast), [MCP server](https://github.com/srini118us/sap-ai-journey/tree/master/mcp-a2a/sap-cashflow-mcp-server) |
| Agentic AP Automation | Supplier invoice processing on SAP BTP | LangGraph, Document AI, S/4HANA | [agentic-ap-automation](https://github.com/srini118us/agentic-ap-automation) |
| Email to Order | Customer PO email to S/4HANA sales order | Google ADK, MCP, S/4HANA, SAP Build Process Automation | [sap-po-demo](https://github.com/srini118us/sap-ai-journey/tree/master/_e2e-candidates/sap-po-demo) |
| Invoice Copilot | Invoice extraction, PO validation, second opinion | LangGraph, GenAI Hub, S/4HANA, Vertex AI | [invoice-copilot](https://github.com/srini118us/sap-ai-journey/tree/master/_e2e-candidates/invoice-copilot) |

## Notes

* Everything runs on personal sandbox and trial environments with synthetic or sample data.
* Each project README documents the problem, architecture, how to run, results, limitations, and next steps.
