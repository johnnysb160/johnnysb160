# Johnny Barros

Senior Software Engineer with 15+ years in technology, building financial, payment, operational, and data-intensive systems where reliability is part of the product.

My professional background includes payment platforms processing more than **R$10M per month**, event-driven services, fraud-prevention flows, financial reconciliation, tax and line-of-business systems, and production delivery across Azure, AWS, Kubernetes, and CI/CD pipelines. I work end to end with **.NET, C#, Blazor, WPF, Entity Framework Core, PostgreSQL, and SQLite**, translating complex business rules into products that operators can understand, trust, and maintain.

The projects below are not tutorial applications. Each one owns a real domain problem, its operational workflow, persistence, failure modes, security boundaries, automated verification, and a deliberate user experience.

## Selected work

### [AppLifePlanner](https://github.com/johnnysb160/AppLifePlanner-Showcase)

A personal operating system that connects the financial ledger to annual planning and daily execution. It manages accounts, cards, transactions, investments, market pricing, fixed income, statement/e-mail imports, reconciliation, annual projections, OKRs, quarterly plans, habits, risks, routines, weekly focus, reviews, vehicles, and a Today action center.

Its central engineering decision is a canonical financial-facts layer: net worth, reserves, contributions, cash flow, and projections are derived once and reused by every planning surface. Owner-scoped PostgreSQL data, encrypted sensitive fields, a persistence-level read-only demo, resilient provider fallbacks, background jobs, paired Windows/iOS companions, Docker, and contract tests turn that product breadth into an operable system.

**Key workflow:** financial activity → canonical facts → annual goals → weekly focus → explainable next actions for today.

`C#` `ASP.NET Core` `Blazor` `EF Core` `PostgreSQL` `WPF` `Docker`

### [TradeGuard](https://github.com/johnnysb160/TradeGuard-Showcase)

A real-operation risk and execution platform for B3 mini futures. It sends and manages actual WDO/WIN orders through MetaTrader 5, supporting operator-led, semi-automatic, and automatic workflows with separate authorization gates for real accounts and strategy automation. The simulator is a validation mode, not the product's identity.

TradeGuard combines a WPF + Blazor Hybrid operator console, deterministic per-instrument engines, 11 scheduled strategies, tape reading, economic-news filtering, position sizing, mandatory stops, break-even, partial exits, trailing and time-based management, portfolio-wide daily/weekly/monthly limits, journaling, replay, parity checks, crash recovery, and end-of-day emergency protection. Its local bridge uses HMAC-SHA256 session authentication, anti-replay sequence numbers, user-only named pipes, DPAPI-backed secrets, and an independent MQL5 safety layer.

**Key workflow:** MT5 market state → serialized decision → portfolio risk gate → protected broker order → management → reconciliation and audit.

`C#` `.NET` `WPF` `Blazor Hybrid` `MQL5` `SQLite` `HMAC`

### [FamilyTree](https://github.com/johnnysb160/FamilyTree-Showcase)

An interactive genealogy system that renders one relationship graph as a multidirectional explorer, an animated lineage treegraph, and a generation-based family tree. Selecting any person rebuilds the point of view and recalculates parents, children, siblings, partners, co-parents, ancestors, descendants, uncles, nephews, and cousins.

The product combines Blazor state and administration with a JavaScript/D3/SVG visualization engine, nearest-common-ancestor kinship calculation, search, shareable focus URLs, remembered selection, responsive zoom/pan and branch controls, a life-event details drawer, contextual relative creation, photo storage, Minimal APIs, EF Core migrations, SQLite, and graph-focused tests. The public repository preserves the complete behavior while replacing the private family history with a fictional dataset and clean history.

**Key workflow:** choose a person → derive relationship graph → visualize from three perspectives → inspect or extend the family record.

`C#` `Blazor` `EF Core` `SQLite` `JavaScript` `SVG`

## Engineering principles

- Model the real business problem before choosing the implementation.
- Make safety rules explicit, testable, and observable.
- Treat privacy and data ownership as product requirements.
- Build interfaces that explain the system's current state and next action.
- Prefer maintainable systems over impressive but fragile demos.

## Professional focus

- Financial and payment systems with auditable transaction lifecycles, reconciliation, fraud controls, and external integrations.
- Clean and event-driven architectures that keep business rules explicit across APIs, messaging, persistence, and user interfaces.
- Operational software designed around failure handling, observability, safe rollout, and decisions that can be explained after the fact.
- Product ownership from discovery and modeling through implementation, automated verification, deployment, and production support.

## What I work with

`C#` · `.NET` · `ASP.NET Core` · `Blazor` · `WPF` · `Entity Framework Core` · `PostgreSQL` · `SQLite` · `Docker` · `GitHub Actions` · `JavaScript`

## Contact

- [LinkedIn](https://www.linkedin.com/in/johnny-b-8154b133/)
- [Email](mailto:johnnysb@gmail.com)
