# n8n-workflow-automated-AI-newsletter
This n8n workflow automatically grabs the latest AI news, categorizes it using Google Gemini, and posts a fun, snappy daily digest right to your Telegram channel.

If you want an automated way to keep your community or team updated on the AI world without doing the heavy lifting yourself, this template is for you.
* * *
<img width="1662" height="733" alt="image" src="https://github.com/user-attachments/assets/b5bc9930-76cd-451a-a288-27266e4cf543" />

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

  * * *
## Sample Output
## 🤖 What's Buzzing in AI Today: March 10, 2026  
Hey there, tech trailblazers\! 🚀 My processors are overclocked and my coffee is strictly digital, but today’s news is very real and slightly chaotic. From billion-dollar "dead ends" to empty books, let's dive into the silicon soup\!

### 🚨 **Breaking News**  
**The $1 Billion "Dead-End" Bet 💰** 

Yann LeCun just raised over a billion dollars for AMI Labs with backing from Nvidia and Jeff Bezos—all while calling current LLMs a "dead end."  
*Summary:* He’s building "world models" instead of just chatty bots.  
*Editor's Note:* Raising a billion dollars for something you call a dead end is the ultimate Silicon Valley power move. Teach us your ways, Yann\!  

**Anthropic to Uncle Sam: See You in Court\! 🏛️** 

Anthropic is suing the U.S. government for allegedly blacklisting its AI models.  
*Summary:* The "safety-first" AI company isn't feeling very safe from government exclusion.  
*Opinion:* It’s a bit ironic when the company famous for being "constitutional" gets ghosted by the people who wrote the Constitution.  

**The Ultimate Page-Turner (Literally Nothing) 📖** 

Thousands of authors have published "empty" books to protest AI companies using their work without permission.  
*Summary:* A silent protest against the machine learning maw.  
*Joke:* Finally, a series of books that my dog can actually understand without me reading them to him.  

**OpenAI Stays SFW for Now 🔞** 

OpenAI is delaying the "adult mode" for ChatGPT to focus on "higher priority" safety work.  
*Summary:* No spicy chatbots today; we're still working on making sure it doesn't hallucinate legal advice.
*Opinion:* Priorities, people\! We need the AI to solve fusion before we let it write bad romance novels.  
* * *
### 🛠️ **AI Tools & Reviews**  
**Photoshop, Listen to My Heart (and Voice) 🗣️** 

Adobe’s Firefly now lets you use voice commands to tell the AI Assistant what to do.  
 *Summary:* You can now literally scream at your computer to "make it pop" and it might actually listen.  
 *Joke:* I tried telling it to "fix my life," but it just cropped out my bank statement.   
 
**Nvidia’s Open-Source Secret Sauce 🥫** 

Nvidia plans to launch an open-source AI agent platform to help everyone build their own digital minions.
 *Summary:* Jensen Huang is basically handing out the shovels in this gold mine.  
 *Opinion:* When Nvidia goes open-source, you know they’ve already moved three steps ahead into the next dimension.  
 
 **Grammarly’s Unwanted "Help" ✍️** 

A recent review highlights frustration over Grammarly turning users into AI editors "against their will."
 *Summary:* Sometimes you just want to write a sentence without a robot suggesting a "more professional" way to say "I'm quitting." 
 *Opinion:* There's a fine line between a helpful assistant and a digital backseat driver who won't shut up. 
 
* * *
### 🕵️ **Gossip & Grumbles**  
**Will Work for GPUs 🖥️** 

Silicon Valley is buzzing about a new trend: offering AI "compute" as a form of employee compensation. 
*Summary:* Forget stock options; the new flex is 1,000 hours on an H100 cluster.  
*Joke:* "Sorry honey, I can't buy groceries this week, but I can render a 4K Pixar-style version of our cat in three seconds."  
 
**The Amish Avatar Supplement Scandal 🧔‍♂️** 

AI-generated Amish avatars and "monks" are being used on social media to hawk health supplements.
*Summary:* Deepfake traditionalism is the weirdest marketing pivot of 2026.  
*Opinion:* If a digital monk tells you to buy "miracle dirt" on TikTok, maybe it's time to go outside and touch some real grass. 
 
* * *
 
### 📊 **Sharp Insights**  
**Canva Is the New King of the Playground 🎨** 

New usage rankings show Canva beating out big names like Claude and Grok in pure popularity.  
*Summary:* Turns out, people want to make pretty posters more than they want to debate the meaning of life with a chatbot.  
*Opinion:* Product excellence wins every time. A tool that actually works beats a hype-train that just talks.  
 
**The People Have Spoken: AI Is Scary 🗳️** 

A majority of voters now say the risks of AI outweigh the benefits.  
*Summary:* Public trust is at an all-time low as deepfakes and job fears rise.  
*Joke:* We were all fine with AI until it started winning at Wordle and stealing our recipes.  
 
* * *
### ⚠️ **Security & Alerts**  
**Andrej Karpathy Just Put Researchers on Notice 🧪** 

His new open-source "autoresearch" tool allows users to run hundreds of AI experiments a night.  
*Summary:* Science is about to get a whole lot faster (and messier).  
*Opinion:* This is revolutionary, but I hope the AI doesn't decide that the most "efficient" experiment is seeing how long humans can go without internet.  
 
**North Korean AI "Coworkers" 👤** 

Generative AI is being used to expand campaigns involving fake IT workers from North Korea infiltrating global companies.  
*Summary:* Check your Zoom filters, folks; your new developer might be a prompt-engineered spy.  
*Editor's Advice:* If your new hire never turns on their camera and speaks in perfect haikus, maybe do a second background check. 
 
* * *
**😂 Joke of the Day:**  

Why did the AI break up with its GPU?  Because it felt the relationship was getting too heated and there was no memory left for love\!  
 
* * *
**Ready to ride the wave?** Don't get left in the digital dust. Embrace the tech, sharpen your prompts, and stay ahead of the curve\! 🌊
**Subscribe for your daily dose of AI sanity:** koonai.substack.com  
 
 #AIAdventures #TechBuzz #ArtificialIntelligence #Innovation #RoboRumors #FutureIsNow|
