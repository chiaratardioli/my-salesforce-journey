# Slackbot AI Sales Planning Assistant

## Overview

This project explored how Slackbot integrates with Salesforce to provide AI-powered sales planning and collaboration capabilities directly within Slack. The implementation demonstrated how conversational AI can retrieve CRM data, summarize opportunities, surface related customer issues, and generate collaborative planning documents without requiring users to leave their communication workspace.

The project focused on integrating Slack with Salesforce CRM and using Slackbot as a context-aware AI assistant for sales preparation, opportunity analysis, and team collaboration.

![Project Overview](./images/ai-02-project-overview.png)

---

## Project Objectives

The primary objectives of this project were:

- Connect Slack with Salesforce CRM securely
- Enable Slackbot access to Salesforce opportunity data
- Prepare and manage CRM opportunity records
- Use conversational AI to retrieve sales insights
- Generate collaborative sales planning documents
- Explore AI-assisted productivity workflows
- Demonstrate secure enterprise AI integration

![Project Objectives](./images/ai-02-project-objectives.png)

---

## Architecture

```text
[ Sales Representative ]
          ↓
[ Slack Workspace ]
          ↓
[ Slackbot AI Assistant ]
          ↓
[ Salesforce CRM Integration ]
          ↓
[ Opportunity & Case Data ]
          ↓
[ AI Analysis & Summaries ]
          ↓
[ Slack Canvas Collaboration ]
          ↓
[ Sales Planning & Team Alignment ]
````

The architecture demonstrated how Slackbot securely accessed Salesforce CRM data and combined it with workplace conversations to support AI-driven sales planning and collaboration workflows.

![Slack Salesforce Architecture](./images/ai-02-slack-salesforce-architecture.png)

---

## Salesforce Technologies Used

* Slackbot AI Assistant
* Slack Playground
* Salesforce CRM
* Agentforce Sales
* Salesforce Opportunities
* Slack Canvas
* Salesforce Integration Framework
* OAuth Authentication
* Salesforce My Domain
* Opportunity Management

![Technologies Used](./images/ai-02-technologies-used.png)

---

## Task 1 — Prepare the Salesforce Environment

I started by creating a new Trailhead Playground environment and retrieving the required Salesforce credentials and domain information needed for the Slack integration process.

I reset the Salesforce password, retrieved the My Domain URL, and prepared the CRM environment for secure authentication between Salesforce and Slack.

I also updated the United Oil Refinery Generators opportunity by extending the close date into the following month so Slackbot would have fresh opportunity data available for analysis.

![Salesforce Environment Setup](./images/ai-02-salesforce-environment-setup.png)

---

## Task 2 — Prepare CRM Opportunity Data

I configured and updated sales opportunity records within Salesforce to simulate a realistic sales planning scenario.

The opportunity data included:

* Opportunity stage information
* Updated close dates
* Customer account details
* Proposal and pricing context

This created a realistic dataset for Slackbot to analyze during the AI-assisted sales planning workflow.

![Opportunity Data Preparation](./images/ai-02-opportunity-data-preparation.png)

---

## Task 3 — Create and Configure the Slack Playground

Next, I created a Slack Playground environment through the Slack Developer Program integrated with Trailhead.

I configured the Slack workspace and prepared the environment for Salesforce CRM connectivity.

This setup enabled the workspace to support:

* Salesforce authentication
* Slackbot AI functionality
* CRM data retrieval
* AI-powered collaboration features

![Slack Playground Setup](./images/ai-02-slack-playground-setup.png)

---

## Task 4 — Integrate Slack with Salesforce CRM

I connected the Slack workspace to Salesforce CRM using Salesforce My Domain and OAuth authentication.

The integration process included:

* Requesting the Salesforce connection from Slack
* Approving the integration within Salesforce Setup
* Activating the CRM connection in Slack
* Granting Slack user access
* Authenticating Salesforce credentials within Slack

This secure connection enabled Slackbot to retrieve Salesforce records and opportunity data directly inside Slack conversations.

![Slack CRM Integration](./images/ai-02-slack-crm-integration.png)

---

## Task 5 — Use Slackbot for Sales Planning

After completing the integration, I tested Slackbot using natural language prompts focused on sales opportunity preparation.

I asked Slackbot to:

* Retrieve open opportunity details
* Summarize account information
* Identify related open support cases
* Generate meeting preparation insights

Slackbot analyzed Salesforce CRM data and returned contextual summaries directly within Slack.

![Slackbot Opportunity Summary](./images/ai-02-slackbot-opportunity-summary.png)

---

## Task 6 — Generate Collaborative Sales Documents

I used Slackbot to transform conversational insights into a structured Slack Canvas document for team collaboration.

The generated canvas included:

* Opportunity summaries
* Key account details
* Open customer issues
* Action items
* Suggested follow-up activities

This demonstrated how AI-generated collaboration documents can help teams coordinate opportunity management and customer engagement workflows.

![Slack Canvas Collaboration](./images/ai-02-slack-canvas-collaboration.png)

---

## Key Features Implemented

* Salesforce and Slack integration
* OAuth-based secure authentication
* AI-powered CRM data retrieval
* Conversational opportunity analysis
* Slack Canvas generation
* AI-assisted meeting preparation
* Context-aware workplace collaboration
* Secure enterprise data access

![Key Features](./images/ai-02-key-features.png)

## Key Skills Demonstrated

* Salesforce CRM integration
* Slack workspace administration
* AI-assisted productivity workflows
* Conversational AI prompting
* Enterprise authentication configuration
* Opportunity management
* AI-driven collaboration tools
* Secure CRM connectivity
* Sales planning workflows
* Cross-platform integration

![Skills Demonstrated](./images/ai-02-skills-demonstrated.png)

---

## Conclusion

This project demonstrated how conversational AI and CRM integration can streamline sales planning and improve team collaboration directly within workplace communication platforms.

Through this implementation, I gained hands-on experience integrating Slack with Salesforce, configuring secure enterprise authentication workflows, and using AI-powered assistants to retrieve, summarize, and organize CRM information.

The project also reinforced how AI assistants can reduce context switching, improve sales preparation efficiency, and support faster decision-making by combining workplace communication with real-time CRM intelligence.


## Resources
- [Trailhead: Get Started with Slackbot](https://trailhead.salesforce.com/content/learn/modules/slackbot-quick-look/get-started-with-slackbot?trailmix_creator_id=teamtrailhead&trailmix_slug=quest-tdx-2026)
- [YouTube: Slack School | Meet Slackbot, Your AI Agent for Work](https://youtu.be/Y_4bX-Bp5s4?si=t_aakET2t6I4Jhh2)
- [Slack Help Center: How to use Slackbot](https://slack.com/help/articles/202026038-How-to-use-Slackbot-%7C-Slack-Help)
- [Slack Developers: Dear Slackbot](https://slack.dev/dear-slackbot/)
