
# n8n Agentic Workflow

This repository contains an n8n workflow for automating interactions between OpenAI models, Gmail, and Google Calendar. The workflow allows users to process chat messages, utilize OpenAI's models for planning and decision-making, and perform actions like sending emails or creating calendar events.

## Workflow Overview

The workflow is designed to process incoming chat messages and perform the following steps:

1. **Chat Message Received**: Triggers when a chat message is received.
2. **OpenAI Planner**: Uses OpenAI models to analyze the message and plan a response or action.
3. **Action Agents**:
   - **GPT-4o Mini**: A smaller OpenAI model for lightweight tasks.
   - **Send Email Tool**: Sends an email via Gmail.
   - **Create Event**: Adds a new event to Google Calendar.
4. **Response**: Finalizes the workflow by sending a manual response.

<img width="1317" alt="Screenshot 2025-01-25 at 2 11 12 PM" src="https://github.com/user-attachments/assets/99916bca-fe99-4fc6-b279-444795e0ca74" />


## Workflow JSON

You can import this workflow into your n8n instance by using the provided `workflow.json` file.

### Importing the Workflow

1. Clone this repository:
   ```bash
   git clone https://github.com/vrajroutu/n8n-agentic-workflow.git
   ```

2. Navigate to your n8n instance.
3. Click on the “Import” button in the workflow view.
4. Select the workflow.json file from this repository.

## Prerequisites

- An active n8n instance.
- API keys or credentials for:
  - OpenAI
  - Gmail
  - Google Calendar
- Properly configured n8n nodes for OpenAI, Gmail, and Google Calendar.

## Setup Instructions

1. **Configure OpenAI**:
   - Set up the OpenAI credentials in your n8n instance.
   - Ensure that the models used (e.g., GPT-4o Mini) are accessible with your API key.
2. **Set Up Gmail and Calendar**:
   - Use the Google credentials node in n8n to authenticate your Gmail and Calendar access.
3. **Test the Workflow**:
   - Trigger the workflow with a sample chat message.
   - Confirm that the email is sent or the calendar event is created as expected.

## Workflow Details

- **Trigger**: When Chat Message Received (Chat)
- **Planner**: OpenAI Planner (Uses OpenAI’s models)
- **Agents**:
  - GPT-4o Mini: Handles lightweight tasks.
  - Send Email Tool: Sends emails.
  - Create Event: Creates Google Calendar events.
- **Response**: Final manual confirmation step.

## Contributing

If you have ideas for improving this workflow or would like to contribute, feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

For more information on n8n workflows, visit n8n.io.
```

Let me know if you need any further adjustments or additional sections!
