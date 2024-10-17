# hello-world-repo


graph TD;
  subgraph Azure_Cloud
    A[User] --> B[Azure Application Gateway]
    B --> C[Azure App Service - Node.js App]
    C --> D[Azure Cosmos DB (MongoDB API)]
    C --> E[Azure Blob Storage]
    F[Azure Monitor] --> C
    F --> D
    F --> E
  end
  
  B -.-> G[Azure CDN]  
  G --> A
