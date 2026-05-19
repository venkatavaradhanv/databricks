# Databricks Power for Kiro

A [Kiro Power](https://kiro.dev/docs) that provides comprehensive Databricks development support with 44 MCP tools (180+ operations) and expert steering files for building data pipelines, ML workflows, dashboards, jobs, and applications on the Databricks platform.

## Installation

Install this Power in Kiro by adding it from the Powers panel using this repository URL:

```
https://github.com/venkatavaradhanv/databricks
```

## What's Included

- **MCP Server** — 44 tools covering SQL, compute, jobs, pipelines, Unity Catalog, dashboards, Genie, model serving, vector search, Lakebase, apps, and more
- **Steering Files** — Expert guidance downloaded from the [Databricks AI Dev Kit](https://github.com/databricks-solutions/ai-dev-kit) during onboarding

## Setup

After installing the Power, activate it in Kiro and follow the onboarding prompts. The setup will:

1. Run the official [Databricks AI Dev Kit installer](https://github.com/databricks-solutions/ai-dev-kit)
2. Download steering files (skills) into the Power's steering directory
3. Configure Databricks authentication

### Prerequisites

- [uv](https://docs.astral.sh/uv/getting-started/installation/) — Python package manager
- git
- A Databricks workspace (AWS, Azure, or GCP)
- [Databricks CLI](https://docs.databricks.com/en/dev-tools/cli/install.html) (optional, needed for OAuth login)

## Authentication Options

- **OAuth login** — `databricks auth login` (requires Databricks CLI)
- **Existing profile** — Use a pre-configured `~/.databrickscfg` profile
- **Personal Access Token** — Direct PAT configuration (no CLI needed)

## Updating Skills

To refresh steering files with the latest from the ai-dev-kit repository, tell Kiro:

```
Update Databricks skills: run the official installer with --tools kiro --global --skills-only --force --silent, then copy skills from ~/.kiro/skills/ to the Power steering directory and clean up.
```

## Resources

- [Databricks AI Dev Kit](https://github.com/databricks-solutions/ai-dev-kit)
- [Databricks Documentation](https://docs.databricks.com)
- [Kiro Documentation](https://kiro.dev/docs)

## License and Support

© 2026 Databricks, Inc. All rights reserved.

The source in this project is provided subject to the [Databricks License](https://databricks.com/db-license-source). The MCP server and skills installed by this Power are sourced from the [databricks-solutions/ai-dev-kit](https://github.com/databricks-solutions/ai-dev-kit) repository and are governed by the same license. See ai-dev-kit's [LICENSE.md](https://github.com/databricks-solutions/ai-dev-kit/blob/main/LICENSE.md) and [NOTICE.txt](https://github.com/databricks-solutions/ai-dev-kit/blob/main/NOTICE.txt) for full terms and third-party attribution.

**Support:**
- Issues with this Power's packaging or installation: [github.com/venkatavaradhanv/databricks/issues](https://github.com/venkatavaradhanv/databricks/issues)
- Issues with the MCP server, skills, or installer: [github.com/databricks-solutions/ai-dev-kit/issues](https://github.com/databricks-solutions/ai-dev-kit/issues)
- Databricks platform support: [help.databricks.com](https://help.databricks.com)
- Privacy: [databricks.com/legal/privacynotice](https://www.databricks.com/legal/privacynotice)
