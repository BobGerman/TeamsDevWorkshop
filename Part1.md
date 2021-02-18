# Building Applications for Microsoft Teams

## Part 1 - Concepts and Low-Code Solutions

| Time | Topics |
|-----|-----|
| 12:30 - 1:45 | Teams, Teams Apps, and SharePoint |
| 1:45 - 2:00 | break |
| 2:00 - 3:00 | Graph, Power Platform, Adaptive Cards |
| 3:00 - 3:15 | break |
| 3:15 - 4:30 | Bots |
_Times are approximate and are in US Eastern Standard Time_

## Slides and Notes

Welcome to Building Applications for Microsoft Teams - Concepts and Low-Code Solutions. This half-day workshop is for anyone who wants to learn how to build applications for Microsoft Teams. It's all about how Teams apps work, backed up with low-code examples. Tomorrow's workshop builds on this one, and goes into the coding aspects of Teams development.

These notes include all the slides and links to relevant resources. You may find it helpful to follow along during the workshop!

![Slide](./Slides/Part1/Slide1-SPFest.PNG)
![Slide](./Slides/Part1/Slide2.PNG)

## What is Teams? What is a Teams app?

To start, let's look at the Teams "Out of the box" experience. Some students may be new to Teams itself, so this is intended to bring everyone up to speed on what's built in.

![Slide](./Slides/Part1/Slide3.PNG)

Microsoft Teams is a brilliant façade over all of Microsoft 365. All of the M365 services are unified into a single user interface in Teams.

![Slide](./Slides/Part1/Slide5.PNG)

A Teams application does not run _in_ _Teams_, it only appears to. Each application is hosted somewhere on the Internet - for example a tab is just a web page, and a bot is a web service. The app package you install into Teams is just a zip file containing a file called manifest.json that tells Teams where these web pages and services are.

![Slide](./Slides/Part1/Slide6.PNG)

The best apps are those that integrate not only with the Teams UI but also with the rest of Microsoft 365. For example, an app that is aware of the user's calendar, or which file a user just edited, can save a lot of steps for the user. The API to access these services is the Microsoft Graph.

![Slide](./Slides/Part1/Slide7.PNG)

Teams app can run anywhere ... except in Teams. They only _appear_ to run in Teams.

![Slide](./Slides/Part1/Slide8.PNG)

Teams apps can run in any of 3 scopes:
 * Teams: App appears in a Teams channel
 * Group Conversation: App appears in a group chat
 * Personal: App appears in the left sidebar or under the "..." for use by individual users

 Some app features work only in specific scopes. For example, a Personal (Static) tab only works in Personal scope; a Configurable tab can run only in Teams or Group Conversations scope. Also Connectors can only work in a Teams channel.

![Slide](./Slides/Part1/Slide9.PNG)

There are many options for extending Teams - you don't necessarily need to write code! This workshop will focus mainly on the Low-Code options; tomorrow will focus on Custom development.

[App Templates](http://aka.ms/TeamsAppTemplates) are pre-written apps that are open source; some are low-code (such as Power Apps) and some are coded solutions that need to be installed in Azure. You can use them as-is or as a starting point for building something new.

![Slide](./Slides/Part1/Slide10.PNG)

The demo continues - now with a custom HR Recruiting app!
The code for the HR sample is [here](https://aka.ms/TeamsHrDevSample). This sample was also part of a workshop; check the [PDF file](https://github.com/OfficeDev/msteams-sample-contoso-hr-talent-app/blob/master/Microsoft%20Teams%20Development%20Bootcamp%20Labs-10-28-2019.pdf) in that repo for instructions (they're not perfect - they're intended to run in a Learning Management System - but you can probably follow them well enough).

![Slide](./Slides/Part1/Slide15.PNG)

Here are some good reasons to build a Teams app!

![Slide](./Slides/Part1/Slide17.PNG)

More useful links:

* [Teams developer documentation](https://aka.ms/TeamsDevDocumentation)
* [Teams developer samples](http://aka.ms/TeamsSampleBrowser)
* [FREE developer tenant!](https://techcommunity.microsoft.com/t5/microsoft-365-pnp-blog/what-is-a-dev-tenant-and-why-would-you-want-one/ba-p/2036610)
* [Hands-on labs (coded in TypeScript)](https://aka.ms/LearnTeamsDev)
* [Teams App Studio](https://aka.ms/InstallTeamsAppStudio)

## Building Apps with SharePoint

![Slide](./Slides/Part1/Slide18.PNG)

Here are the details on [Learning Pathways](https://docs.microsoft.com/en-us/office365/customlearning/) including setup instructions.

[Here are step-by-step instructions](http://aka.ms/SPPagesAsTeamsApps) for making Learning Pathways (or any SharePoint site) into a Teams app.

![Slide](./Slides/Part1/Slide19.PNG)

Here is the blog article [SharePoint and Teams: Better Together](https://techcommunity.microsoft.com/t5/microsoft-sharepoint-blog/sharepoint-and-teams-better-together/ba-p/189593) that goes with this demo!

![Slide](./Slides/Part1/Slide20.PNG)

Teams are based on [Microsoft 365 Groups](https://support.microsoft.com/en-us/office/learn-about-microsoft-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) so you can count on having a SharePoint site, Outlook calendar etc. for every Team.

Another helpful article is [Microsoft 365 Groups and Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/office-365-groups). And an awesome article and infographic from MVP [Matt Wade](https://www.jumpto365.com/author/matt-wade): [An Everyday Guide to Microsoft Office 365 Groups](https://www.jumpto365.com/blog/everyday-guide-to-office-365-groups)

![Slide](./Slides/Part1/Slide21.PNG)

Notice that nearly everything ends up in Exchange or SharePoint so all those compliance features can be used!

![Slide](./Slides/Part1/Slide22.PNG)

If you're a licensed user of Teams, check out your OneDrive and you'll see the folders!

![Slide](./Slides/Part1/Slide23.PNG)
* [Global Developer Bootcamp 1: Building Teams Apps with SharePoint](https://aka.ms/Bootcamp1Lab)
* [Teams Tabs in SharePoint Framework](http://bit.ly/TeamsSPFx)
* [Field visit tab sample](https://aka.ms/360DegreeCollab)

## Building Apps with Power Apps

![Slide](./Slides/Part1/Slide24.PNG)
![Slide](./Slides/Part1/Slide25.PNG)

* [Power Apps as Tabs](https://aka.ms/PowerAppsTeams)

## Adaptive Cards with Power Automate

![Slide](./Slides/Part1/Slide27.PNG)
![Slide](./Slides/Part1/Slide29.PNG)

* [Adaptive Cards](https://adaptivecards.io/)

![Slide](./Slides/Part1/Slide30.PNG)

* [Use Adaptive Cards in Power Automate](https://docs.microsoft.com/en-us/power-automate/create-adaptive-cards)


## Building an App with Graph Toolkit

![Slide](./Slides/Part1/Slide31.PNG)
![Slide](./Slides/Part1/Slide32.PNG)

* [Microsoft Graph Explorer](https://bit.ly/GraphExplorer)
* [MS Graph Postman Collection](https://bit.ly/GraphPostman)
* [Azure AD Postman Collection](https://bit.ly/AadPostman)

![Slide](./Slides/Part1/Slide33.PNG)
![Slide](./Slides/Part1/Slide34.PNG)

* [Graph Toolkit article and sample](https://aka.ms/CallGraphTeamsTab-GraphToolkit)
* [Global Developer Bootcamp 2: Building Teams Apps with Graph Toolkit](https://github.com/OfficeDev/M365Bootcamp-TeamsOneProductivityHub)

## Webhooks and Connectors

![Slide](./Slides/Part1/Slide35.PNG)

* [Incoming and Outgoing Webhooks](https://aka.ms/TeamsWebhooks)
* [Building Custom Connectors](https://docs.microsoft.com/en-us/MicrosoftTeams/office-365-custom-connectors)

## Building Bots

![Slide](./Slides/Part1/Slide38.PNG)
![Slide](./Slides/Part1/Slide39.PNG)
![Slide](./Slides/Part1/Slide40.PNG)

Try Eliza [here](http://plnkr.co/edit/MGIjQ3mEEpiOOXivA0zz?preview) and even play with the source code!

![Slide](./Slides/Part1/Slide41.PNG)
![Slide](./Slides/Part1/Slide42.PNG)

* [QnA Maker](https://www.qnamaker.ai/)

![Slide](./Slides/Part1/Slide44.PNG)
![Slide](./Slides/Part1/Slide45.PNG)
![Slide](./Slides/Part1/Slide46.PNG)
![Slide](./Slides/Part1/Slide47.PNG)
![Slide](./Slides/Part1/Slide48.PNG)

* [Power Virtual Agents](https://aka.ms/PowerVirtualAgent)
* [Azure Bot Framework Composer](https://aka.ms/CallGraphFromBot)
* [LUIS (Language Understanding Intelligent Service](https://www.luis.ai/)
* [Consulting bot sample](https://aka.ms/ConsultingBotSample)

![Slide](./Slides/Part1/Slide49.PNG)
![Slide](./Slides/Part1/Slide50.PNG)



