# SWiki

A simple, collaborative wiki platform that organizes knowledge as a graph of interconnected concepts, enabling users to create, 
link, and explore information in a more semantic and structured way.

## High-Level Requirements

- Support collaborative article creation and editing.
- Store knowledge in a graph structure (nodes and edges) rather than flat documents.
- Enable semantic linking between articles to represent relationships.
- Provide keyword search across the knowledge base.
- Offer visual graph navigation to explore connections between concepts.
- Maintain version history for articles with rollback options.
- Implement role-based access control for reading and editing.
- Expose a query API for programmatic graph exploration.
- Ensure scalability for large, interconnected knowledge sets.
- Support schema evolution to add new relationship types over time.

## Feature Roadmap

### MVP (Phase 1) – Core Foundations

- User Accounts & Authentication (basic login/registration).
- Article Management: create, edit, delete articles.
- Semantic Linking: articles can link to other articles as structured relationships.
- Keyword Search across articles.
- Basic UI: article editor + simple graph visualization.
- Version History (basic): track edits, rollback to previous versions.

### Phase 2 – Collaboration & Structure

- Role-Based Access Control: define permissions (admin, editor, viewer).
- Advanced Graph Navigation: interactive visualizations with filters and zooming.
- Rich Content Support: images, attachments, embedded media.
- Tagging & Categorization for articles.
- Notifications: changes, mentions, and collaboration updates.

### Phase 3 – Scalability & Extensibility

- Schema Evolution Support: ability to add new relationship types and attributes without breaking existing data.
- Advanced Querying: natural language search mapped to graph queries.
- Integration Hooks: import/export data (Markdown, CSV, RDF, JSON-LD).
- Analytics & Insights: most linked articles, knowledge gaps, usage metrics.
- Mobile-Friendly UI for browsing and editing.

### Phase 4 (Future / Stretch Goals) – Intelligence & Automation

- AI-Assisted Linking: suggest relationships between concepts automatically.
- Ontology Management: define controlled vocabularies and hierarchies.
- Recommendation Engine: suggest related articles or missing links.
- Knowledge Validation Rules: enforce constraints on certain relationships.

## Core Tech Stack

Core Runtime

- Aspire .NET 9 based solution for easy start up and developer experience.
- Azure Function for backend logic with scalable cost-effective API.
- Blazor WebAssembly for frontend.
- Testing with XUnit, FluentAssertions, NSubstitute and BUnit (front end)
- Podman for local development running Gremlin Server for Graph Database and SQL server for generate database (e.g. auth)
- Production cloud infrastructure replaces Gremlin Server with Azure Cosmos DB (Graph API) and SQL server with Azure SQL server.