# Slackbot AI Productivity Assistant

This project explored how Slackbot uses conversational AI and workplace context to improve productivity and collaboration inside Slack. Slackbot acts as an AI-powered work assistant capable of searching conversations, summarizing discussions, retrieving information, and helping users prepare for meetings and daily tasks.

Through this module, I learned how Slackbot integrates with enterprise systems such as Salesforce to provide context-aware assistance while maintaining strict security and permission controls.

## Key Capabilities Explored

- Summarizing conversations and missed updates
- Retrieving important files and messages
- Preparing meeting overviews using Slack and Salesforce data
- Generating action plans and organized summaries
- Supporting lead follow-up and customer engagement workflows
- Performing contextual analysis across workplace conversations

## Skills Demonstrated

- Conversational AI understanding
- AI-assisted workplace productivity
- Context-aware prompting
- Salesforce and Slack ecosystem integration
- Enterprise AI security awareness
- Workflow optimization and collaboration tools

## Prepare the data

- Create a new playgroung and get the pwd and the url domain
- Open the opportunity United Oil Refinery Generators in stage *Proposal/Price Quote* and changed the close date to next month.

Learning Objectives
After completing this unit, you’ll be able to:

Update opportunity data in Agentforce Sales.
Integrate Agentforce Sales with Slack.
Use Slackbot to help you bring Salesforce data into the flow of work.
Before You Start
Before you start this badge, consider completing this recommended content.

Slackbot: Quick Look
Bring CRM Context to Slack
If you completed Slackbot: Quick Look, you learned how Slackbot simplifies work by helping with tasks like preparation for important meetings. As your AI agent for work, Slackbot gathers context from threads, channels, and Salesforce records so you don’t have to switch tools.

To enable this powerful productivity feature, you must connect Slack with Salesforce. When you integrate Salesforce and Slack, Slackbot reads and displays record details directly in your chat window. It connects information across accounts and opportunities and helps users make smarter decisions.

In this badge, you work through a scenario where you prepare data for an upcoming deal renewal—which mirrors a use case from Slackbot: Quick Look.

Ready to Get Hands-on with Agentforce Sales and Slackbot?
Follow along and complete the steps in this badge to create both a Trailhead Playground and a Slack Playground.

Let’s start by creating a brand-new Trailhead Playground in this unit. Scroll to the bottom of this page, click the playground name, and then select Create Playground. It typically takes 2–3 minutes for Salesforce to create your Trailhead Playground.

Note: Yes, we really mean a brand-new Trailhead Playground! If you use an existing org or playground, you can run into problems completing the steps in this badge.

Get Your Trailhead Playground Username and Password
Let's get started by opening your Trailhead Playground. Scroll to the bottom of this page and click Launch. Follow the steps below to get your Trailhead Playground username and reset the password.

With your Trailhead Playground open, click the Get Your Login Credentials tab and take note of your username.
Click Reset My Password and then Ok. This sends an email to the address associated with your username.
Click the link in the email.
Enter a new password, confirm it, and click Change Password.
Note: For quick reference later, you can paste your Trailhead Playground username in the element below, and it will appear in a similar element when you need it in the next unit. This information is temporarily stored in your browser for this session only and is not sent anywhere else.


Retrieve Your Domain URL
When you integrate with Slack in the next unit, you need your My Domain URL to kick off the authentication process. It’s good to get this information now. Here’s how to do it in your brand-new Trailhead Playground.

Click setup icon and select Setup.
In the Setup Quick Find, search for and select My Domain.
Copy the URL in the Current My Domain URL field somewhere handy. It should be in this format: (your-domain-name)-dev-ed.trailblaze.my.salesforce.com.
Note: For quick reference later, you can paste your unique domain URL in the element below, and it will appear in a similar element when you need it in the next unit. This information is temporarily stored in your browser for this session only and is not sent anywhere else.


Prepare Your Sales Data
Now, give Slackbot something to talk about.

Click App Launcher icon to open the App Launcher, select the Sales app.
Click the Opportunities tab.
Update the list view to All Opportunities.
Locate the opportunity United Oil Refinery Generators in the Proposal/Price Quote stage.
Click the pencil icon next to the close date for this opportunity.
Update its close date to some time next month of this year.
Click Save.
You now have a fresh opportunity ready for Slackbot to analyze.

Keep Your Agentforce Sales Playground Open
Great work! In the next unit, you create a Slack Playground and connect it to this Trailhead Playground. It’s best to have these playgrounds open in separate tabs so you can accomplish the integration with ease.



## Integrate Slack with CRM

Operate with Trust and Security
Slackbot operates under strict security standards and respects the running user’s existing Salesforce permissions. It only surfaces CRM data the user is authorized to view. To establish this secure connection, you add the Agentforce Sales and Agentforce Service apps to Slack and authenticate your user account.

Note
Do You Already Have a Slack Playground?
To complete this badge, you need to have a Slack Playground provisioned from Trailhead. If you don’t have a Slack Playground yet, proceed to the section, Retrieve Your Trailhead Slack Playground.

If you already have a Slack Playground, scroll to the bottom of the page, and launch your playground from the Hands-on Challenge section.

From the dropdown, select your email address.
Click Connect Slack Playground.
Then click Launch.
Your Slack Playground is ready!
Now complete the section, Request a Connection to Salesforce.
Retrieve Your Trailhead Slack Playground
Trailhead is integrated with the Slack Developer Program. This enables us to provide you with a special Slack Playground designed for hands-on learning. When you connect your Trailhead account to Slack for the first time, you’re signed up for the Slack Developer Program, which gives you access to a wealth of Slack development resources.

It’s time to get your Slack Playground up and running.

Scroll down to the Challenge section of this page, where it says Hands-on Challenge.
By default, your primary Trailhead email address is selected. If you prefer another email address that’s associated with your Trailhead account, click on the email dropdown and select it.
Add a check to the box next to “I accept the Slack Developer Terms of Service.” Optionally, you can check the next box to subscribe to the Slack Developer Newsletter.
Authorization window for Slack Playground with email field, terms checkbox, and Create Slack Playground button.

Click Create Slack Playground. After a moment, your playground is created and the page refreshes.
Scroll back down to the challenge section. Click Launch to open your playground in a new tab.
Connected email account learningfun@gmail.com with Disconnect Slack Playground and Launch buttons.

The first time you open your playground, a terms of service modal appears. Click I Agree.
Your Slack Playground is ready!

Request a Connection to Salesforce
Now you can connect your Salesforce org to Slack. When you request a Salesforce connection in Slack, you can choose how your members’ Slack and Salesforce accounts connect. You have the option to automatically configure member accounts using Email or SAML NameID fields. For this badge, you manually configure user accounts using your admin credentials. Remember the domain URL you retrieved from your CRM org in the previous unit? You use it in this section.

In your Slack Playground, click the down arrow next to your workspace name to view the dropdown menu.
Dropdown arrow next to the workspace name highlighted.

Note: Your workspace name differs from the image.

Navigate to Tools & settings | Manage Salesforce Organizations. This takes you to the Salesforce organizations page.
Manage Salesforce Organizations menu selection.

Note: This opens the Slack admin page in an additional tab. Keep both Slack tabs open.

Click the Connect Salesforce Org button.
Paste the domain URL into the field for Salesforce org to connect.
Note: If you added your domain URL to the form in unit 1, simply copy the text from the element below. After copying your username, click Clear. You no longer need this information.


Uncheck the toggle for Map user accounts automatically. Keep all other options as is.
Click Request Connection. You get a response that the request was sent to the Salesforce admin. That’s you!
Click Okay.
The integration is now underway. Next, you accept the connection on the Salesforce side.

Accept the Connection
Head back to your Trailhead Playground. Once the request to connect has been made in Slack, a Salesforce admin (in this case, you!) can approve it in Salesforce.

Return to your Trailhead Playground tab.
Click setup icon and select Setup.
In the Setup Quick Find, search for and select Manage Slack Connection.
Click the checkbox to the Agree to terms, including the Slack user terms.
Click Approve. The connection page refreshes, and the Waiting for activation by Slack admin status appears.
Manage Slack Connection window with Approved Connection and the Waiting for activation by Slack admin status.

Activate the Connection in Slack
Now it’s time to head back to Slack and finalize the connection. Workspace owners and Salesforce admins can activate a pending Salesforce connection.

Return to the Slack admin tab you have opened from the previous section and refresh the page. Your Salesforce org appears with a Connection status of Ready to activate.
Note: If you closed the Slack admin page tab, open your Slack playground and click Workspace name | Tools & settings | Manage Salesforce organizations to re-open the Slack admin page.

In the Connection status column, click View details.
Slack window open to Salesforce organizations with view details link highlighted.

Click Activate.
In the modal, click Activate.
Stay on this page for the next step.

Add Your Slack User to Salesforce
Next, add your Slack user.

Click the Users tab.
Click Add individually.
In the Salesforce org window under the Users tab, the Add individually link is highlighted.

In the search bar, type youcopy, and select the Slack user with “(you)” at the end.
Click Grant Access to 1 Person.
Under the Users tab, your Slack user is now listed.

Sign Your Slack User into CRM from Slack
The final part of this integration is to sign in using your CRM (Trailhead Playground) org credentials.

Head back to your Slack workspace (the other Slack tab). If you kept the tab open, refresh.
In the navigation, click Sign in to Salesforce.
Slack interface with the Sign in to Salesforce button highlighted.

Click Continue.
Click Continue to Salesforce.
Enter the username for your Trailhead Playground, and paste it into the Salesforce login username.
Note: If you added your Trailhead Playground username to the form in unit 1, simply copy the text from the element below. After copying your username, click Clear. You no longer need this information.


Enter the password you created.
Note
If you accidentally closed the modal, you can always navigate to an alternative sign-in page via your workspace name | Preferences | Salesforce.
Click Login then Allow.
Click Done.
You get a message that you successfully connected your account. You can close the OAuth window. Click back into your Slack workspace, and the modal shows that your org is connected. Now that you have successfully connected your Trailhead Playground to your Slack workspace, it’s time to see Slackbot in action.

Note
Do You Have Multiple CRM Orgs Connected?
You may get an error in the Challenge section of this badge if you have multiple CRM orgs connected to your Slack playground. Make sure you only have the org related to this badge connected.

Click the down arrow next to your workspace name.
Go to the admin dashboard: Click Tools & settings | Manage Salesforce Organizations
Click … next to the CRM org you wish to disconnect.
Select Disconnect org.
Then, click Disconnect.

## Ask Slackbot to Help with a Sales Meeting
Prepare for an Important Meeting
You created your customer records in Salesforce and authenticated your Slack workspace. Now it’s time to put Slackbot to work.

In this scenario, you act as a sales rep who’s preparing for a big renewal meeting. You need to review the opportunity you prepared in the first unit.

You do not need complex commands to interact with Slackbot—just talk to it using simple, natural language.

Within your Slack Playground, click Slackbot at the top of the screen.
Slack Playground with Slackbot icon highlighted.

Enter the prompt: Find the open united oil refiner generators opportunity and summarize the details.copy
Press enter/return. Slackbot searches your Salesforce records and returns the opportunity details.
Enter the prompt: I’m preparing for a team meeting to discuss this opportunity. Are there any open cases we should be aware of that might need our attention?copy
Press enter/return to send your prompt to Slackbot. Slackbot cross-references the account with any open cases.
You have the information you need. Now, save it so your team can review it. Slackbot turns conversational queries into structured documents using Slack Canvases.

Tell Slackbot: Turn this information into a canvas called UO Oppty Brief, please call out key details and action items so the team can swarm and keep the opportunity green.copy
Press enter/return to send your prompt to Slackbot. Slackbot creates the canvas.
Open the canvas to make sure it captures the information you asked for. Try adding a cover image, and additional details you’d like to share with the team.
You’re fully prepared for your meeting, and your team is aligned.


## Conclusion

With a secure connection between Slack and your CRM (in this case, your Trailhead Playground), Slackbot combines your sales and service data with 
the operations and conversational context found in Slack. This unlocks smarter deal planning. And you don’t have to swivel between apps to get it.

This project demonstrated how AI assistants can reduce time spent searching for information, improve collaboration efficiency, and help teams make faster, more informed decisions using existing workplace data and communication history.

The experience also strengthened my understanding of how AI-powered assistants are being integrated into modern enterprise platforms to support daily business operations and customer-focused workflows.


## Resources
- [Trailhead: Get Started with Slackbot](https://trailhead.salesforce.com/content/learn/modules/slackbot-quick-look/get-started-with-slackbot?trailmix_creator_id=teamtrailhead&trailmix_slug=quest-tdx-2026)
- [YouTube: Slack School | Meet Slackbot, Your AI Agent for Work](https://youtu.be/Y_4bX-Bp5s4?si=t_aakET2t6I4Jhh2)
- [Slack Help Center: How to use Slackbot](https://slack.com/help/articles/202026038-How-to-use-Slackbot-%7C-Slack-Help)
- [Slack Developers: Dear Slackbot](https://slack.dev/dear-slackbot/)
