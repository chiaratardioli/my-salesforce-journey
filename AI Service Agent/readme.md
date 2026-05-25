# AI-Powered Service Agent with Salesforce Agentforce Builder

## Overview

This project demonstrates the creation of an AI-powered customer service agent using Salesforce Agentforce Builder. The agent was designed for Coral Cloud Resorts to help customers learn about resort experiences, validate customer information, retrieve available sessions, and create bookings through conversational interactions.

The implementation combined Salesforce Flow automation, AI-driven reasoning, Experience Cloud integration, and embedded messaging to deliver an interactive customer support solution.

![Customer Conversation Demo](./images/AI-01-customer-conversation-demo-1.png)

---

## Project Objectives

The agent was designed to support the following customer service tasks:

- Provide information about resort experiences and activities
- Validate customer identity using email and membership number
- Retrieve available experience sessions
- Book customer reservations directly through Salesforce
- Deliver a conversational support experience through Experience Cloud

---

## Architecture
```AI-Service-Agent-Architecture
[ Experience Cloud UI ]
          ↓
[ Embedded Messaging ]
          ↓
[ Agentforce AI Layer ]
          ↓
[ Subagents + Actions ]
          ↓
[ Flow Builder ]
          ↓
[ Salesforce CRM Data ]
```

---

## Technologies Used

### Salesforce Components

- Agentforce Builder
- Agentforce Studio
- Salesforce Flow Builder
- Experience Cloud
- Embedded Messaging
- CRM Data Objects
- Subagents and Custom Actions

### AI Features

- Conversational AI workflows
- Instruction-based agent reasoning
- AI-assisted configuration
- Action orchestration
- Dynamic conversation handling

---

## Creating the Service Agent

The first step involved creating a new service agent inside Agentforce Studio.

### Agent Configuration

- Agent Name: `CC Service Agent`
- Role: Customer service representative
- Purpose: Assist resort guests with reservations and activity information

The agent was configured with access permissions using the EinsteinServiceAgent user profile.

![Service Agent Setup](./images/AI-01-service-agent-setup.png)

---

## Exploring Agentforce Builder

Agentforce Builder provided three primary areas for development:

### Navigation Explorer

Used to manage:
- Settings
- Subagents
- Variables
- Connections
- Data Sources

### Editor View

Supported:
- Canvas View
- Script View

### Agentforce Assistant

Used natural language prompts to update instructions and configuration.

![Agentforce Builder Interface](./images/AI-01-agentforce-builder-interface.png)

---

## Creating the Experience Management Subagent

A dedicated subagent named `Experience Management` was created to handle all customer requests related to resort activities and experiences.

### Responsibilities

- Answer experience-related questions
- Retrieve activity details
- Manage reservations
- Handle session selection

![Experience Management Subagent](./images/AI-01-experience-management-subagent.png)

---

## Creating Custom Actions

Custom actions were configured to allow the AI agent to interact with Salesforce data and flows.

### Get Experience Details

This action retrieved information about resort experiences.

#### Features

- Connected to Salesforce Flow
- Required customer context
- Returned experience information to the conversation

![Get Experience Details Action](./images/AI-01-get-experience-details-action.png)

![Get Experience Details Input Action](./images/AI-01-get-experience-details-action-inputs.png)

---

### Get Customer Details

This action validated customer identity using:
- Email address
- Membership number

The action returned the related Salesforce Contact record.

![Get Customer Details Action](./images/AI-01-get-customer-details-action.png)

---

## Adding Actions from the Asset Library

Two reusable actions were imported from the Salesforce Asset Library:

- Get Sessions
- Create Experience Session Booking

These actions allowed the AI agent to:
- Retrieve available activity sessions
- Create booking records directly in Salesforce

![Asset Library Actions](./images/AI-01-asset-library-actions.png)

---

## Configuring Agent Instructions

The subagent instructions defined how the AI should behave during customer interactions.

### Instruction Logic

The agent was configured to:
1. Validate the customer before performing actions
2. Retrieve experience details when requested
3. Request missing information when needed
4. Retrieve sessions using experience IDs
5. Create bookings with selected sessions and guest counts

![Subagent Instructions](./images/AI-01-subagent-instructions.png)

---

## Using Script View

Script View allowed direct editing of the agent instructions and logic.

Additional booking instructions were added manually to improve session booking behavior and data handling.

![Script View Editing](./images/AI-01-script-view-editing.png)

---

## Activating and Testing the Agent

After configuration, the agent version was committed and activated.

The Preview functionality was used to test:
- Customer validation
- Experience information retrieval
- Session lookup
- Reservation creation

Example customer interaction:

> "Can you let me know more about the full moon beach party experience?"

The agent requested customer verification before retrieving information and booking sessions.

![Agent Preview Testing](./images/AI-01-agent-preview-testing-1.png)
![Agent Preview Testing](./images/AI-01-agent-preview-testing-2.png)
![Agent Preview Testing](./images/AI-01-agent-preview-testing-3.png)
![Agent Preview Testing](./images/AI-01-agent-preview-testing-4.png)

Since Live Test Mode was enabled, the agent executed real transactions in the Salesforce org. As a result, a booking was created for Sofia Rodriguez, confirming an experience reservation scheduled for May 25, 2026.

![Agent Live Test Data](./images/AI-01-agent-live-test-data.png)


---

## Publishing the Experience Cloud Integration

The agent was integrated into the Coral Cloud Experience Cloud website using Embedded Messaging.

### Deployment Steps

- Published Embedded Service Deployment
- Updated the routing flow to the service agent
- Added the messaging component to the site

![Experience Cloud Integration](./images/AI-01-experience-cloud-integration-ESD.png)
![Experience Cloud Integration](./images/AI-01-experience-cloud-integration-routing.png)
![Experience Cloud Integration](./images/AI-01-experience-cloud-integration-site.png)

---

## Customer Experience Demonstration

Customers interacted with the AI agent directly through the Experience Cloud website, simulating a real-world customer support and booking scenario.

### Supported Capabilities

- Ask about resort experiences  
- Verify account details  
- View available sessions  
- Complete activity bookings  

The conversational workflow provided a guided customer support experience that was fully connected to Salesforce CRM data and automated backend processes.

![Customer Conversation Demo](./images/AI-01-customer-conversation-demo-2.png)

Below is the updated Salesforce Contact record for Sofia Rodriguez after the booking was completed through the website interaction.

![Booking Confirmation](./images/AI-01-booking-confirmation.png)

---

## Key Skills Demonstrated

### Salesforce Skills

- Agentforce Builder
- Flow Builder
- Experience Cloud
- Embedded Messaging
- CRM Integration
- AI Agent Configuration

### AI and Automation Skills

- Conversational AI
- Instruction Engineering
- Workflow Automation
- AI Action Orchestration
- Customer Service Automation

---

## Conclusion

This project demonstrated how Salesforce Agentforce can be used to build intelligent AI-powered customer service solutions integrated directly into CRM workflows.

By combining conversational AI, Salesforce Flows, custom actions, and Experience Cloud deployment, the solution provided an end-to-end customer support and reservation management experience.

The implementation also highlighted the importance of AI instruction design, secure customer validation, and workflow orchestration when building enterprise AI agents inside the Salesforce ecosystem.

---

## References

1. [Trailhead: Build with Agentforce Builder](https://trailhead.salesforce.com/content/learn/modules/quick-start-assemble-a-service-agent-with-agentforce-builder/build-with-agentforce-builder?trailmix_creator_id=teamtrailhead&trailmix_slug=quest-tdx-2026)

2. [Salesforce Help: Create Agents in Record Time with Agentforce Implementation Guides](https://help.salesforce.com/s/articleView?id=ai.agent_resources.htm&type=5)

3. [Website: Salesforce AI Use Case Library](https://www.salesforce.com/artificial-intelligence/use-cases/)

4. [Agentforce Developer Guide: Agent Script Reference](https://developer.salesforce.com/docs/ai/agentforce/guide/ascript-reference.html)
