# n8n-workflow-automated-AI-newsletter
This n8n workflow automatically grabs the latest AI news, categorizes it using Google Gemini, and posts a fun, snappy daily digest right to your Telegram channel.

If you want an automated way to keep your community or team updated on the AI world without doing the heavy lifting yourself, this template is for you.
* * *

## What It Does
1. **Fetches Daily News**: Pulls the latest updates from three Google News RSS feeds (Generative AI, AI Platforms, and general AI topics).
2. **Filters Out the Old**: Automatically filters the feed so it only processes news published today.
3. **Cleans the Data**: Strips out messy HTML tags so the AI gets clean, readable text.
4. **Smart Categorization**: Uses Google Gemini (Gemini 3.0 Flash) to act as an editor. It sorts the raw news into clear groups: News, Review, Gossip, Insight, and Alert.
5. **Writes the Newsletter**: A second Gemini agent (Gemini 3.0 Flash) steps in as a witty copywriter. It takes the categorized news and writes an engaging digest with emojis, short summaries, and a daily joke.
6. **Posts to Telegram**: Sends the final, formatted digest directly to your Telegram chat or channel.
* * *
## Prerequisites
To use this workflow, you need a few things set up in your n8n instance:

- **Google Gemini API Key**: Needed to run the AI Classifier and Copywriter agents.
- **Telegram Bot Token**: Needed to send the final message.
- **Telegram Chat ID**: You need the specific ID of the channel or group where you want the bot to post.
* * *
## How to Set It Up
1. Copy the JSON code of this workflow.

2. Open your n8n workspace, click Add Workflow, and paste the JSON directly into the canvas.

3. Open the Google Gemini Chat Model nodes and connect your Google API credentials.

4. Open the Telegram node and connect your Telegram API credentials.

5. In the Telegram node, swap out the default chatId (-1001126995747) with your own.

6. Click Test Workflow to make sure everything runs smoothly.

7. Toggle the workflow to Active. By default, it runs every day at 10 AM.
* * *
## Make It Your Own
You can easily tweak this template to fit your exact needs:

- **Change the Schedule**: Double-click the Schedule Trigger to change the time or frequency.

- **Track Different Topics**: Open the RSS Feed Read nodes and replace the Google News URLs with feeds for your own industry (crypto, finance, sports, etc.).

- **Change the Tone**: Open the Copywriter📝 node and edit the System Message. You can tell the AI to be highly professional, sarcastic, or brief depending on your audience.

- **Update the Call to Action**: Currently, the prompt includes a link to koonai.substack.com. Be sure to update this in the Copywriter node to point to your own newsletter or website!
