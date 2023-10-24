
## 👋 Hello World 
🤘 Hi everyone! I'm David from 🌶️ [Chili Shelf](https://www.chilishelf.com), and I'm super thrilled to show you what we've been working on for this Codegeist'23 (our first one!)
  
## 💡 Inspiration 
I think it's fair to say that many people were blown away when we saw Chat GPT 🤯. At least for me, it was a jaw-drop moment. The possibilities seemed endless. So you can imagine what my reaction was when Open AI made their APIs public:

![My reaction after testing Chat GPT](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/blown-away.gif)
> I HAVE to get my hands on this. NOW!

Is the tech cool? Yes. Is there some hype to it? Maybe. Can it solve every single problem in the world? Absolutely not. 
So, I wanted to check it first hand. I started to incorporate AI into my life. From Google searches to basic questions to coding assistance, data processing, data analysis, image/asset generation and.. of course, **Jira** Too ❤️

After using LLM for almost a year, I see **many** real-world applications for LLM (Large Language Models), like Chat GPT, to increase productivity, foster innovation and have more information at our fingertips faster.  All of those things **go beyond the classic TL; DRs (text summaries).**   The more you use LLMs, the more you understand it is all about '*how you use it'*. To the point that even a new profession came from it, the so-called [Prompt Engineering](https://en.wikipedia.org/wiki/Prompt_engineering).

It became clear to me that whatever we build using an LLM needs to have a **human input and guidance** and be as transparent as possible. That will be a recurrent theme. AI, without human guidance, tends to go off the rails or even [hallucinate](https://en.wikipedia.org/wiki/Hallucination_%28artificial_intelligence%29). 

It is not *us vs them* (or at least I hope so..😥). It is not AI reading your mind and fully anticipating what you want (at least, just yet). It is AI + humans. *#StrongerTogether*

![Humans + AI - Stronger together! (generated with Dall-E 3](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/humans_ai_450px.png)


### Our app design convictions 
To sum it up, we wanted to build an app that would take the following into account:

 - **🤖 👨‍💻 AI + Humans.** Users need to be able to enrich answers provided by AI.
 - 🛠️ **Customisable**. We don’t know everything and we can’t predict how users could find different ways to interact with Chat GPT. Let them decide how.
 - 🎨 **UX at its core**. Needs to be easy and intuitive to use. Also need to feel integrated with Jira and follow the Atlassian Design system as much as we can.
 - 🔍 **Data Transparency**. Be clear about what EXACTLY is sent over.
 - ❌ **It is NOT magic**. Explain to users that it cannot be fully relied upon. And it does make mistakes.
 - 💸 **API requests cost money**. Don't hide it, but also be able to monitor it.
  - 👀 **Visibility**. Not everyone needs to have access to this.
 - 🌊 **It's evolving, so expose it**. Expose Chat GPT settings so the site admins can better adapt it to their liking
 



## 🤔 What it does 
(**drumroll*\*) 🥁

### 👉 **Introducing 🤖 GPT Insights for Jira** 👈

![TL;DR](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/summary.png)
> A cloud-only Atlassian forge app that allows your Jira users to get direct insights from Chat GPT in order to supercharge their day-to-day operations⚡.

 🤖 GPT Insights for Jira integrates with [OpenAI](https://openai.com/)'s Chat GPT and lets your Jira users run different prompts using the issue `description` and `comments` as input. 

It integrates directly into whatever task, ticket or epic it is needed in AND can run prompts based on comments too. It takes the form of a small modal with concise UI so it's extremely intuitive and easy to use.

 They can choose from a variety of customisable prompts. ie:
-   📝 Summary, bullet point summarization
-   🔍 Key topics, list the main key topics in the following text
-   🎯 Next steps, suggest next actions based on the text
-   ❓ Find ambiguities, identify ambiguous points in the text
-   🧠 Simplify the current text, produce a jargon-free text
-   😄 Sentiment analysis (identify the sentiment of the text)



![Wait... there's more!](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/wait-theres-more.jpeg)

We also have more advanced functionalities:
- 💡 Custom user prompts
- 📝 Edit message responses
- 💬 Chat Assistant
- 📊 Usage Stats
-  🛡️ Group visibility settings
- ⚠️ User and data transparency & AI Transparency


### 🌶️ Spicy features
We love to stay spicy, so get ready...! 🔥🧑‍🚒

###  💡 Insights
Managed by the site admin. These are the list of the default prompts available to all users with access to the app. They run the top of the UI as tabs that you can use to run a prompt with a single click.

![Identify stakeholders](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/insights-stakeholders.png)

In the app settings, you can edit and add prompts within the table. Settings include:

 - Tab Name
 - Prompt
	 - Query to Chat GPT:  `Prompt` + ( `Ticket description` OR `ALL aggregated comments` )
 - Answers in bullets / full sentences
 - Priority / in-tab list (the first tab gets called first)
 - Enabled / Disabled

![Global prompts](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/settings_prompt.png)

### 🪄 **Custom user prompts** 

Here, users can define their own (private) prompts, which work across all issues, so each time they open a new Jira issue, they have quick access to it.

Simply write your prompt, give it a name and hit save. These prompts are stored and saved in tabs across the top of the modal within the Custom Tab, just like the Insights Tab.


![Trimp-ify, because... why not?](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/custom_prompt-trumpify.png)

### 📝 Edit message responses

⚠️ **Chat GPT makes mistakes and may give inaccurate responses.** That's why we introduced the option for users (managed by the site admin in the app settings) to manually edit and enrich messages. 

![Edit by humans](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/edited-message.png)

The bar at the top shows who made edits to the answer last and when (icon tooltip). The surrounding blue box will turn purple when showing an edited response. 

There's also a toggle that can show the original ai-generated response so users can see what exactly was altered if need be.

In the app settings, you can actually turn this feature on/off as well as control which user groups have the ability to edit responses.

![Message settings](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/admin_messages-settings.png)




###  💬 **Chat Assistant.**

Why does it have to be one-way? If you have more questions, just "chat with your ticket". We have an Insights Assistant, AI-powered, that will help you. 

Also, it will remember the context of your previous questions so you can ask about something and keep expanding on it and getting more specific. Just as you would on ChatGPT itself.


![Chat against your own data](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/chat.png)

### 🔃 **Smart caching (pay for what you need 🤑)**
There's no need to keep sending the same question over and over again. Especially when you have to pay for each request. That's why we implemented '*smart caching*' that stores the response for as long as the ticket hasn't changed.  ie: 
> User1 opens Issue ID X-123 and requests the 'Next steps'. Two days pass, and User2 opens the same issue and clicks on 'Next steps'. Unless the description/comments have changed, we won't make a new open API request. Hence. the request will be at $0.

![Optimise costs with caching](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/caching.png)

### 💸 **Usage stats**
With great power comes a great responsibility. But with an API that costs money per request... we better keep things in check! That's why we introduce a usage page, where we can see:

- How many users use the app
- How much have we spent in total
- How much we saved because of caching vs having fresh/new responses
- Who uses the app, how much have they spent so far and when did they use it last.

![enter image description here](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/usage.png)


### ⚠️ **User and data transparency & AI Transparency** 
This is critical. We expose EXACTLY what has been sent to OpenAI, which model we used, how many tokens have been consumed, and how much it costs.
Also, we remind the user Open AI's data policies to both admin and users. Providing even a FAQ in the admin section so the admin has a full understanding of how the app works.

![Data transfer](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/data-transfer-info.png)
![Disclaimer](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/disclaimer.png)
![FAQ](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/faq.png)

### 🛡️ **Group visibility settings**
We understand that each Jira instance is its own world. Not everyone might need to have access to this. That's why we can control who (user groups) can access the app.

![Visibility settings](https://chili-shelf-public.s3.eu-north-1.amazonaws.com/visibility_settings-only.png)



## 🛠️ How we built it 
For the forge app, we used custom UI with typescript, tailwind, atlaskit, vite.js + hot reloading, prettier and vscode as IDE. 


###  Documentation:
We kept our eyes glued to these pages during the development of the apps.

- Forge doc https://developer.atlassian.com/platform/forge
- Atlaskit doc for UI components- https://atlassian.design/components/
- Atlassian Design tokens to make our app compatible with the Atlassian Design system as well as their themes (Dark/light mode) - https://atlassian.design/components/tokens/all-tokens
- Atlassian Forge dev community - https://community.developer.atlassian.com/c/forge/
- For everything OpenAI related, we used their [API playground](https://platform.openai.com/playground?mode=chat) 
 

### Forge setup
When it comes to developing forge apps, 🔥 **hot reloading is super important** to make your (dev) life MUCH easier. I couldn't stress it enough. 🥵
Big props to *Oliver Siebenmarck* from [polymetis](https://www.polymetis-apps.com/) 🙇‍♂️. He shared his forge+customUI+vite.js+hot-reloading boilerplate project in this [public repo](https://bitbucket.org/oliversiebenmarck/forge-vite-template/src/main/). 

That helped us a lot. We discovered this in his talk  `Ludicrous Speed Speed up Development with Forge Tunnel and Vite`. If you want to know more, you can check it in youtube [here](https://www.youtube.com/watch?v=YNc-JQIjNcQ).



### Additional libraries we used
- lottiefiles for the svg gif animations 
	- https://www.npmjs.com/package/@lottiefiles/react-lottie-player
- confetti-explosion-react
	- https://www.npmjs.com/package/react-confetti-explosion


### Manifest.yml file
This is the backbone of the app. Where you connect the dots for Atlassian when deploying your app. Here are some of the more relevant things we used.

#### Forge module
We used the following modules:
- **jira:issuePanel**. GPT Insights Jira issue button. This will use the Jira `description` as input for the Chat GPT query.
- **jira:issueActivity**. GPT Insights Jira activity button (next to the comments section). This will use ALL the  `comments` as input for the Chat GPT query.
- **jira:adminPage**. Admin page. Where the Open AI key and the rest of the GPT Insights settings, usage and FAQ are.

#### Triger events
Due to our '*smart caching*' we needed to **detect when an issue changed** so we could invalidate the cache and request a new request. 
We used triggers for that. One for the issue and another for the comments. All are linked to a function that, on update would flag the `issueId_promptID` as obsoleted. 

    trigger:
       - key: issue-updated-event
          function: updated
          events:
             - avi:jira:updated:issue
             - avi:jira:commented:issue

#### External 
We rely on OpenAI's Chat GPT API. We had to declare our app would be fetching external requests (outside Atlassian infrastructure).

    external:
	   fetch:
	      backend:
	      - api.openai.com




#### Scopes
In order to make all this magic happen, you need access to different aspects of the Jira instance where the app will be installed. Forge has this secure scope system (similar to your phone and other services), so on-install, the admins know **exactly** what they are giving access to.

    scopes:
       - write:jira-work
       - read:jira-user
       - read:jira-work
       - storage:app

-   **write:jira-work**: For storing user preferences and their custom insights to user properties.
-   **read: jira-user**: For accessing user details such as display name, avatars and group roles.
-   **read:jira-work**: For accessing jira issue description and comment information to send to OpenAI.
-   **storage:app**: For storing admin preferences and responses from ChatGPT.


### Autoconsent
This one is fresh out of the oven! **We finally have autoconsent in preview** 🤩. If this is not added, each user has to approve the app individually. That would be shown as an approval message on the app iframe redirecting them to a different Atlassian page where they would see the scope the app is accessing to. 
This would happen the first time they use it.

With this app feature on, after the admin installs the app, it can be fully utilised by everyone without explicit consent.

    app:
       features:
          autoUserConsent: true




## 🤦‍♂️ Challenges we ran into 
This is the list of some of the challenges we ran into during the development of the hackathon.

- **Forge tunnel** is not as stable as we'd have liked... Sometimes, it would not work, or it would cache some stuff. That's the worst because it drives you crazy. 
	- When this happened, we relied on the good ol' full deployment. But that made the development more painful since that can take up to ~20-40 sec
- **Implementing cached responses** was a challenge to work out the best way to structure prompts/responses data both for descriptions and comments
- We wanted to **stream the responses** like the actual Chat GPT does, but we couldn't do it due to the current `node runtime` limitations. 
	- 📢 I'm happy to say that the new node runtime seems to be now in [preview](https://developer.atlassian.com/platform/forge/runtime-reference/native-nodejs-runtime/) at the time of this writing, so this might be different now! 
 - **Theme compatibility**. This is always challenging. You have to make sure that your assets and components look OK when in light/dark mode. That's why sticking to the ADS is key. Although, there's always the need for more and you end up creating your own components.
 - **Responsive design**. We had to take into account how things would look like if you resize the issue frame. Also, due to the nature of jira, the app can be opened from different places/views.
 - Issues with the **modal module.** We had some problems where buttons where exceeding the actual container. We end up just having a larger view so that would be sorted out.

## 💪 Accomplishments that we're proud of 
- 📝 **Edit responses**. We really believe in this AI + Human theme. And this is a good example of that. Also, we like the concept of living the 'ticket better than you found it'.
	- Also, that edited/original toggle shows you what has also changed. So we keep the integrity of the original message, too.
-  🔃 **Smart caching**. We are very happy with how this turned out. This was one of our main concerns when creating an app heavily relying on a paid API. Implementing this makes it more cost efficient. Technically was also really cool to come up with the right data structures that would make querying more efficient.

- 💬 **Live chat**. Talking '*with*' your ticket. That is its own section. We like the possibilities it can bring. Particularly useful for long tickets or long comment threads. We also added some `system` constraints, so the assistant will only answer the questions if they are around the ticket and make sense in the ticket context.
- 📊 **Usage stats**. We love data, we like stats. Being able to monitor what has been spent in total  and how it's being used it's important.

- 💡 **Custom prompts**. Letting that door open for user's creativity it's great. I'm sure many new examples of this will come out. Our favourite so far is the Trump-ify, or rewrite the ticket as a short riddle. Summarising in 5 words is cool too.

- 🎨 **UI & UX**. After many hours in & out of figma, and several iterations, we are quite happy the attention to detail we put in different aspects of the app. From tooltips, to submenus, internal navigation, inner modals, etc.  
	- The *get started page* wizard, makes the process of setting up the app much easier. Walking through the user how to obtain an API key and make sure it's a valid one with a test button.



## 🤓 What we learned 

- Our body can take more **coffee** ☕ than we anticipated.
- We learnt more about the **latest Chat GPT API's**, and LLMs in general. How they work, and their pros and cons. What they are good at and bad at.
- We became more familiar with the Atlassian Design System and the **tokens design** 🎨.
- We learn different ways of how to **leverage the storage API** to store different data structures.
- The **dev community is the go-to place** when you get stuck! We've got so many useful tips and got nudged in the right direction many times. Can't stress it enough. If you are stuck on something, chances are someone else has been there too.
- Become more familiar with **triggers and issue events**.
- ... and that machines are not our enemy. Yet 👀




## 🚀 What's next for GPT Insights for Jira?
There's still a looooot to do! Things in our roadmap:
- Using the **new node runtime engin**e to implement response streaming.
- Chat GPT **Model tuning** with custom data.
- **Smart Actions**. ie: Create each bullet point of the next steps list into child tasks. Or update/enrich ticket summary using AI.
- Better integration with jira (jira @user tags), highlight `dates` and an improved response **message formatting**.
- **Share responses** in different channels (slack, teams, email)
- **More usage stats** (week/month/year usage, user analytics, etc.)
- A **JSM** version for the 'public'.
- **Advanced budgeting**. Per user and group usage limits.
- ...and much more! 🚀🌑


💡 Have you got any other suggestions..? Write us at support@chilishelf.com we are always happy to discuss ideas and new features! 😍


## 🙏 Thank you! 
Phew..!! I know. It is a long one..! 🙄 But you can always summarize it, right? ha!

Thanks so much if you made it this far. I just really wanted to capture our journey building the app. I found myself on the other end many times, reading the 'how it was done', and I took so much from them, so I figured it would be just fair to do the same and give back in case it might be interesting to someone else 😄


Stay fresh, stay spicy! 🌶️


David. out. 🎤



