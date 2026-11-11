# Awesome-Cloud-Data-Migration-Seeding

## Top Cloud Data Migration & Seeding Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Workload Migration, Database Seeding & Large-Scale Data Transfer*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Data Migration & Seeding**. These tools help organizations move workloads, databases, mailboxes, and file shares from on-premises or legacy environments into the cloud—covering server replication, application migration, mailbox transfers, and synthetic data seeding for development and testing environments.

**Examples** include Druva Data Migration, AWS Application Migration Service, Azure Migrate, Google Cloud Migration Center, Fivetran, Matillion, BitTitan MigrationWiz, Carbonite Migrate, Zerto Cloud Migration, Quest Migration Manager, and Datadobi (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted database migration, schema seeding, and data transfer tooling—ideal for data engineers, platform teams, and developers seeking transparent, vendor-neutral migration infrastructure without per-TB or per-mailbox licensing surprises.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global cloud migration services market is estimated at **$300B–$325B in 2025** and projected to reach **$380B–$405B in 2026** (growing at an ~18–25% CAGR), with the dedicated data migration software and tooling subset accounting for **$11.3B–$12.8B**. 

The sector features a **hybrid market structure**: it is **heavily concentrated at the top** around the core hyperscalers (Microsoft Azure, AWS, Google Cloud) and global systems integrators capturing major platform workloads, yet **moderately-to-highly fragmented across specialized migration software, database transformation tools, and niche workload movers** where independent SaaS vendors compete on protocol support, minimal downtime cutovers, and compliance.

## SaaS/Hosted Platforms

| Product | Company Valuation / Revenue Scale | Description | Pricing (Starting Tier) | Free Tier / Trial Limits |
|---------|-----------------------------------|-------------|------------------------|--------------------------|
| **[Azure Migrate](https://azure.microsoft.com/en-us/products/azure-migrate/)** | ~$4.0T Market Cap (Microsoft) | Microsoft's migration hub for discovering, assessing, and migrating on-premises servers, databases, and web apps to Azure. | **$25.00/month per server** (after initial 180-day free replication window; assessment tools are free, standard Azure runtime resources billed separately) | **Free for the first 180 days per replicated server**; discovery and TCO assessment hub are permanently free (underlying Azure storage/compute billed as consumed) |
| **[Google Cloud Migration Center](https://cloud.google.com/migration-center)** | ~$3.4T Market Cap (Alphabet) | Unified platform for assessing and migrating on-premises workloads to Google Cloud. Provides discovery, TCO analysis, and migration planning for VMs, databases, and containers. | **$0 base software fee** (free migration discovery & assessment; pay-as-you-go Compute Engine / Cloud Storage rates apply upon workload cutover) | **Permanently free assessment & planning platform** with no metered agent limit; new GCP accounts receive **$300 free trial credits for 90 days** |
| **[AWS Application Migration Service](https://aws.amazon.com/application-migration-service/)** | ~$2.9T Market Cap (Amazon) | Lift-and-shift server migration to AWS with continuous block-level replication. Install replication agent on source servers, launch test/cutover instances in AWS. | **$0.042/hour per server** (~$30/month per active server after 90 days; staging EC2/EBS infrastructure billed separately) | **90-day free tier per source server** (2,160 hours of continuous replication per agent) |
| **[Zerto Cloud Migration](https://www.zerto.com/)** | ~$60B Market Cap (HPE, acquired for $374M) | Continuous data replication for cloud migration and disaster recovery. Supports VMware, Hyper-V, and Azure VMware Solution with journal-based recovery (RPO seconds, RTO minutes). | **$700–$1,000/VM per year** (starting tier migration license through HPE/partner channel; Enterprise Cloud Edition lists at ~$1,400–$2,200/VM/year) | **14-day to 30-day free trial** (typically capped at 10 to 15 virtual machines for evaluation) |
| **[Carbonite Migrate](https://www.carbonite.com/)** | ~$6.2B Market Cap (OpenText, acquired for $1.42B) | Server migration and replication tool (formerly Double-Take Move) for moving physical, virtual, and cloud workloads with minimal downtime. | **$275.00 one-time per source server** (Carbonite Migrate Standard 60-day node-locked license; Premium 90-day license at ~$495/server) | **30-day proof-of-concept / evaluation license** (available via OpenText sales/partners; consumer backup offers 15-day trial, server migration requires evaluation key) |
| **[Fivetran](https://www.fivetran.com/)** | ~$5.6B Valuation (~$300M+ ARR) | Managed ELT platform with 700+ connectors for database and SaaS data migration into warehouses. Usage-based on Monthly Active Rows (MAR). | **$5.00/month minimum base** ($5 base for up to 1M MAR, prorated at ~$495/million MAR thereafter on Standard pay-as-you-go) | **Permanent Free Plan up to 500,000 MAR/month** (plus 3,500 reverse-ETL MAR and 5,000 model runs/month); **14-day full-access trial** with unlimited sync volume on initial connector setups |
| **[Quest Migration Manager](https://www.quest.com/)** | ~$5.4B Valuation (Clearlake Capital, ~$500M ARR) | Suite for Microsoft 365, Active Directory, and Exchange migrations. Handles coexistence, directory synchronization, and mailbox migration for enterprise environments. | **~£16–£36 ($20–$46)/user per year** (starting Tier 1 volume pricing on Quest On Demand Migration; module add-ons start at ~£4.90/object) | **30-day free trial** capped at **5 user accounts/mailboxes** (max 5 GB per mailbox, 256 MB per OneDrive account, and 5 SharePoint sites up to 5 GB each) |
| **[BitTitan MigrationWiz](https://www.bittitan.com/)** | ~$3.0B Parent Valuation (Idera, Inc.) | SaaS-based mailbox, document, and Teams migration platform. Supports Microsoft 365 tenant-to-tenant, Google Workspace, Exchange, and hybrid migrations. | **$14.00 per mailbox license** (single mailbox up to 50 GB data limit; User Migration Bundle at $17.50 for unlimited data/OneDrive) | **Free trial migration pass** with **unlimited runs**, capped strictly at **10 items per folder** and **5 MB total data per mailbox** |
| **[Druva Data Migration](https://www.druva.com/)** | ~$2.0B Valuation (~$200M+ ARR) | Cloud-native data protection and migration for endpoints, servers, and SaaS workloads. Supports migration to new laptops, M365 tenants, and cloud infrastructure with global deduplication. | **$4.00/user per month** (starting tier for endpoint/M365 migration; server data volume backup/migration starts at ~$200/TB-month) | **30-day free trial** (up to 30-day extension cap; full platform evaluation without credit card upfront) |
| **[Matillion](https://www.matillion.com/)** | ~$1.5B Valuation (~$99M ARR) | Cloud-native ELT with push-down transformation to Snowflake, Databricks, Redshift, and BigQuery. Billed per credit consumption (task hours). | **$2.00–$2.50 per credit** (~$1,000/month baseline spend; orchestration consumes ~1 credit/hour, transformation consumes ~3 credits/hour) | **14-day free trial** with **500 complimentary platform credits** (full connector and pipeline access, no disabled core features) |
| **[Datadobi](https://www.datadobi.com/)** | ~$10M–$50M ARR (Bootstrapped Private) | Unstructured file and object data migration, storage assessment, and lifecycle management platform (StorageMAP / DobiMigrate). | **$30,560.00/year** (AWS Marketplace 100 TB base annual subscription for StorageMAP data management; add-on migration modules quoted by capacity) | **30-day customized PoC / evaluation license** (enterprise proof-of-concept arranged via direct sales/partners; no self-serve public tier) |

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
