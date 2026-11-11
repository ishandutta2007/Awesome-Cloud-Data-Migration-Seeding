# Awesome-Cloud-Data-Migration-Seeding

# Top Cloud Data Migration & Seeding Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Workload Migration, Database Seeding & Large-Scale Data Transfer*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Data Migration & Seeding**. These tools help organizations move workloads, databases, mailboxes, and file shares from on-premises or legacy environments into the cloud—covering server replication, application migration, mailbox transfers, and synthetic data seeding for development and testing environments.

**Examples** include Druva Data Migration, AWS Application Migration Service, Azure Migrate, Google Cloud Migration Center, Fivetran, Matillion, BitTitan MigrationWiz, Carbonite Migrate, Zerto Cloud Migration, Quest Migration Manager, and Datadobi (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted database migration, schema seeding, and data transfer tooling—ideal for data engineers, platform teams, and developers seeking transparent, vendor-neutral migration infrastructure without per-TB or per-mailbox licensing surprises.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Druva Data Migration](https://www.druva.com/)** | Cloud-native data protection and migration for endpoints, servers, and SaaS workloads. Supports migration to new laptops, M365 tenants, and cloud infrastructure with global deduplication and agentless backup . | Quote-only (custom pricing; 4 tiers: Business, Enterprise, Elite, Productivity Data)  | No free tier available; trial via sales [citation:1] |
| **[AWS Application Migration Service](https://aws.amazon.com/application-migration-service/)** | Lift-and-shift server migration to AWS with continuous block-level replication. Install replication agent on source servers, launch test/cutover instances in AWS. Free for 90 days (2,160 hours) per server from agent installation . | Free for 90 days per server; thereafter billed hourly per server during active replication. Additional AWS infrastructure (EC2, EBS, data transfer) billed separately [citation:2][citation:10] | **90-day free tier per source server** (2,160 hours), sufficient for most migrations [citation:2] |
| **[Azure Migrate](https://azure.microsoft.com/en-us/products/azure-migrate/)** | Microsoft's migration hub for discovering, assessing, and migrating on-premises servers, databases, and web apps to Azure. Includes Server Migration, Database Migration, and Web App Migration tools. | Free tool; pay only for Azure resources consumed (VMs, storage, networking) | Free assessment and migration tooling; Azure consumption costs apply |
| **[Google Cloud Migration Center](https://cloud.google.com/migration-center)** | Unified platform for assessing and migrating on-premises workloads to Google Cloud. Provides discovery, TCO analysis, and migration planning for VMs, databases, and containers. | Free assessment tooling; pay for GCP resources consumed | Free assessment and planning; GCP consumption costs apply |
| **[BitTitan MigrationWiz](https://www.bittitan.com/)** | SaaS-based mailbox, document, and Teams migration platform. Supports Microsoft 365 tenant-to-tenant, Google Workspace, Exchange, and hybrid migrations. User Migration Bundle covers mailbox, archives, OneDrive, and Google Drive . | Mailbox: $14 (50 GB limit); User Migration Bundle: $17.50 (unlimited data); Public Folders: $114 per 10 GB [citation:3] | Free MigrationWiz account to purchase online; new customer offer: Buy 2, get 1 free on User Migration Bundle (up to 100 free licenses) [citation:3] |
| **[Carbonite Migrate](https://www.carbonite.com/)** | Server migration and disaster recovery tool for moving physical, virtual, and cloud workloads with minimal downtime. Supports cross-hypervisor and cross-cloud migrations. | From ~$219 one-time (per SelectHub analysis; pricing varies by scope) [citation:4] | No free trial per SelectHub listing; demo available [citation:4] |
| **[Zerto Cloud Migration](https://www.zerto.com/)** | Continuous data replication for cloud migration and disaster recovery. Supports VMware, Hyper-V, and Azure VMware Solution with journal-based recovery (RPO seconds, RTO minutes). Enables test migrations without production impact. | Quote-only (subscription per protected VM; varies by term and volume) | Trial available via sales; no self-serve free tier |
| **[Quest Migration Manager](https://www.quest.com/)** | Suite for Microsoft 365, Active Directory, and Exchange migrations. Handles coexistence, directory synchronization, and mailbox migration for enterprise environments. | From ~$100–$500 annually (per SelectHub range; custom quote required) [citation:6] | Free trial available; no permanent free tier [citation:6] |
| **[Datadobi](https://www.datadobi.com/)** | Unstructured data migration and storage management platform. Moves file shares and object storage between on-premises and cloud environments with metadata preservation and integrity verification. | Quote-only (enterprise contract) | Trial via sales; no self-serve free tier |
| **[Fivetran](https://www.fivetran.com/)** | Managed ELT platform with 700+ connectors for database and SaaS data migration into warehouses. Usage-based on Monthly Active Rows (MAR); initial syncs excluded. | Pay-as-you-go (Standard); $5 minimum per connection generating 1–1M MAR | Free plan: no base charge, 5,000 monthly model runs for transformations |
| **[Matillion](https://www.matillion.com/)** | Cloud-native ELT with push-down transformation to Snowflake, Databricks, Redshift, and BigQuery. Billed per credit (task hour): 1 for orchestration, 3 for transformation. | Credit-based; ~$2.00/credit (third-party listing) | No free tier; demo via sales |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[dbferry](https://github.com/AbdLim/dbferry)** | [![Stars](https://img.shields.io/github/stars/AbdLim/dbferry?style=social&color=white)](https://github.com/AbdLim/dbferry/stargazers) | Local-first database migration tool for PostgreSQL, MySQL, SQLite, and more. No telemetry, no external calls; schema + data migration with resumable checkpoints and checksum verification. YAML config, optional FastAPI web UI. Apache 2.0 [citation:8] |
| **[pgloader](https://github.com/dimitri/pgloader)** | [![Stars](https://img.shields.io/github/stars/dimitri/pgloader?style=social&color=white)](https://github.com/dimitri/pgloader/stargazers) | PostgreSQL-focused data loading and migration tool. Migrates from MySQL, SQLite, MS SQL, and CSV to PostgreSQL with schema conversion, error handling, and parallel loading. |
| **[Flyway](https://github.com/flyway/flyway)** | [![Stars](https://img.shields.io/github/stars/flyway/flyway?style=social&color=white)](https://github.com/flyway/flyway/stargazers) | Database schema migration and seeding tool. Version-controlled SQL migrations across PostgreSQL, MySQL, Oracle, SQL Server, and more. Community edition free; Teams/Enterprise paid. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Liquibase](https://github.com/liquibase/liquibase)** | [![Stars](https://img.shields.io/github/stars/liquibase/liquibase?style=social&color=white)](https://github.com/liquibase/liquibase/stargazers) | Open-source database schema change management. Supports XML, YAML, JSON, and SQL changelogs across major databases. Community edition free. |
| **[dbt Core](https://github.com/dbt-labs/dbt-core)** | [![Stars](https://img.shields.io/github/stars/dbt-labs/dbt-core?style=social&color=white)](https://github.com/dbt-labs/dbt-core/stargazers) | SQL-based transformation and seeding framework for data warehouses. Handles the "T" in ELT and supports seed files for reference data. |
| **[Apache NiFi](https://github.com/apache/nifi)** | [![Stars](https://img.shields.io/github/stars/apache/nifi?style=social&color=white)](https://github.com/apache/nifi/stargazers) | Dataflow automation and migration tool with visual interface. Supports routing, transformation, and mediation between systems with provenance tracking. |

**Frameworks for building custom systems**: Combine **dbferry** for local-first cross-database migration, **Flyway** or **Liquibase** for schema versioning and seeding, and **dbt Core** for warehouse transformations—creating a fully self-hosted data migration and seeding pipeline without per-mailbox or per-TB licensing.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Data migration tools handle sensitive production data; enforce encryption in transit, least-privilege source credentials, and audit logging for all migration jobs.
- Migration pricing models vary widely (per-server, per-mailbox, per-TB, custom quote); model total cost against actual data volume and cutover timeline before committing to annual contracts.

---

**Made for data engineers, platform teams, migration architects, and developers building data movement infrastructure.**  
Let's make cloud data migration and seeding more open, verifiable, and cost-predictable.
