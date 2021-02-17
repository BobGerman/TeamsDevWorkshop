# Building Applications for Microsoft Teams

## Part 2 - Deeper Dive and Developer Solutions

### Approximate Schedule

| Time | Topics |
|-----|-----|
| 12:30 - 1:45 | Review, Hello World, SharePoint Framework |
| 1:45 - 2:00 | break |
| 2:00 - 3:15 | Bots, Adaptive Cards, Messaging Extensions |
| 3:15 - 3:30 | break |
| 3:30 - 4:30 | Calling Microsoft Graph from your Teams app |

## Slides and Notes

Welcome to Building Applications for Microsoft Teams - Deeper Dive and Developer Solutions. This half-day workshop is for anyone who wants to learn how to build applications for Microsoft Teams. It's all about how Teams apps work, backed up with low-code examples. Tomorrow's workshop builds on this one, and goes into the coding aspects of Teams development.

These notes include all the slides and links to relevant resources. You may find it helpful to follow along during the workshop!

![Slide](./Slides/Part2/Slide1-SPFest.PNG)
![Slide](./Slides/Part2/Slide2.PNG)

## Review: Teams Apps and App Manifest

Microsoft Teams is a brilliant façade over all of Microsoft 365. All of the M365 services are unified into a single user interface in Teams.

![Slide](./Slides/Part2/Slide3.PNG)

A Teams application does not run _in_ _Teams_, it only appears to. Each application is hosted somewhere on the Internet - for example a tab is just a web page, and a bot is a web service. The app package you install into Teams is just a zip file containing a file called manifest.json that tells Teams where these web pages and services are.

![Slide](./Slides/Part2/Slide4.PNG)

The best apps are those that integrate not only with the Teams UI but also with the rest of Microsoft 365. For example, an app that is aware of the user's calendar, or which file a user just edited, can save a lot of steps for the user. The API to access these services is the Microsoft Graph.

![Slide](./Slides/Part2/Slide5.PNG)
![Slide](./Slides/Part1/Slide10.PNG)

There are many options for extending Teams - you don't necessarily need to write code! This workshop will focus mainly on the Low-Code options; tomorrow will focus on Custom development.

[App Templates](http://aka.ms/TeamsAppTemplates) are pre-written apps that are open source; some are low-code (such as Power Apps) and some are coded solutions that need to be installed in Azure. You can use them as-is or as a starting point for building something new.

![Slide](./Slides/Part2/Slide6.PNG)
![Slide](./Slides/Part2/Slide7.PNG)

Teams apps can run in any of 3 scopes:
 * Teams: App appears in a Teams channel
 * Group Conversation: App appears in a group chat
 * Personal: App appears in the left sidebar or under the "..." for use by individual users

 Some app features work only in specific scopes. For example, a Personal (Static) tab only works in Personal scope; a Configurable tab can run only in Teams or Group Conversations scope. Also Connectors can only work in a Teams channel.

### More helpful links:
* [Teams developer documentation](https://aka.ms/TeamsDevDocumentation)
* [Teams developer samples](http://aka.ms/TeamsSampleBrowser)
* [Hands-on labs (in TypeScript)](https://aka.ms/LearnTeamsDev)
* [Teams App Design guidance](http://bit.ly/Design4Teams)

## Hello, World: Creating your project

![Slide](./Slides/Part2/Slide9.PNG)

* [Yo Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/tutorials/get-started-yeoman)
* [Teams Toolkit for VS Code and Visual Studio](https://aka.ms/TeamsToolkitVS)

* [Teams App Studio](https://aka.ms/InstallTeamsAppStudio) - Manifest editor runs right in Teams

![Slide](./Slides/Part2/Slide10.PNG)
![Slide](./Slides/Part2/Slide11.PNG)

## Tabs with SharePoint Framework

![Slide](./Slides/Part2/Slide12.PNG)
![Slide](./Slides/Part2/Slide13.PNG)

* [Overview of the SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview)

![Slide](./Slides/Part2/Slide14.PNG)
![Slide](./Slides/Part2/Slide15.PNG)
![Slide](./Slides/Part2/Slide16.PNG)
![Slide](./Slides/Part2/Slide17.PNG)
![Slide](./Slides/Part2/Slide19.PNG)
* [Teams Tabs in SharePoint Framework Tutorial](http://bit.ly/TeamsSPFx)
* [Global Developer Bootcamp 1: Building Teams Apps with SharePoint](https://aka.ms/Bootcamp1Lab)
* [Field visit tab sample](https://aka.ms/360DegreeCollab)

## Bots with Azure Bot Framework

![Slide](./Slides/Part2/Slide20.PNG)
![Slide](./Slides/Part2/Slide21.PNG)

* [Azure Bot Framework](https://dev.botframework.com/)
* [Bot Framework SDK - v3 vs. v4](https://docs.microsoft.com/en-us/azure/bot-service/migration/migration-about)

![Slide](./Slides/Part2/Slide22.PNG)
![Slide](./Slides/Part2/Slide23.PNG)

If you want to see the generated code without running the generator, there's a copy [here](https://github.com/BobGerman/Bots/tree/master/Templates)

![Slide](./Slides/Part2/Slide25.PNG)
![Slide](./Slides/Part2/Slide26.PNG)

If you want to see the generated code without running the generator, there's a copy [here](https://github.com/BobGerman/Bots/tree/master/Templates

![Slide](./Slides/Part2/Slide29.PNG)

* [Azure Bot Framework Emulator](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-debug-emulator)
* [ngrok](https://ngrok.com/)
* [Azure remote debugging](https://docs.microsoft.com/en-us/visualstudio/azure/vs-azure-tools-debug-cloud-services-virtual-machines)

![Slide](./Slides/Part2/Slide30.PNG)
![Slide](./Slides/Part2/Slide31.PNG)

* [Setting SSL for local tab debugging](https://bob1german.com/2020/10/17/setting-up-ssl-for-tabs-in-the-teams-toolkit-for-visual-studio-code/)

![Slide](./Slides/Part2/Slide32.PNG)
![Slide](./Slides/Part2/Slide33.PNG)

* [State Bot](https://github.com/BobGerman/Bots/tree/master/StateBot)

![Slide](./Slides/Part2/Slide34.PNG)
![Slide](./Slides/Part2/Slide36.PNG)
![Slide](./Slides/Part2/Slide37.PNG)

* [Bot Dialogs documentation](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-concept-dialog?view=azure-bot-service-4.0)

![Slide](./Slides/Part2/Slide38.PNG)
![Slide](./Slides/Part2/Slide41.PNG)

* [LUIS (Language Understanding Intelligent Service](https://www.luis.ai/)

![Slide](./Slides/Part2/Slide42.PNG)
![Slide](./Slides/Part2/Slide43.PNG)

More Bot Links

* [Bob's Bot Workshop at last year's SPFest!](https://github.com/BobGerman/Bots)
* [QnA Maker](https://www.qnamaker.ai/)
* [Bot Builder Quickstart](http://bit.ly/AzBotBuilder)
* [Consulting bot sample](https://aka.ms/ConsultingBotSample)

## Adaptive Cards deeper dive

![Slide](./Slides/Part2/Slide44.PNG)
![Slide](./Slides/Part2/Slide46.PNG)
![Slide](./Slides/Part2/Slide47.PNG)
![Slide](./Slides/Part2/Slide48.PNG)
![Slide](./Slides/Part2/Slide49.PNG)
![Slide](./Slides/Part2/Slide50.PNG)
* [Adaptive Cards](ttps://adaptivecards.io/)

## Messaging Extensions

![Slide](./Slides/Part2/MsgExt1.PNG)

* [What are Messaging Extensions](https://docs.microsoft.com/en-us/microsoftteams/platform/messaging-extensions/what-are-messaging-extensions)

![Slide](./Slides/Part2/MsgExt2.PNG)
![Slide](./Slides/Part2/Slide51.PNG)

* [Build a Messaging Extension](https://docs.microsoft.com/en-us/microsoftteams/platform/build-your-first-app/build-messaging-extension)
* [Building Messaging Extensions with SPFx](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/build-for-teams-expose-webparts-teams)
* [Northwind customers sample](https://github.com/pnp/teams-dev-samples/tree/master/samples/msgext-customer-search)
* [HTTP Status Cats](https://knowyourmeme.com/memes/http-status-cats)
* [HTTP Status Cats messaging extension](https://github.com/pnp/teams-dev-samples/tree/master/samples/msgext-httpstatuscats)

## Calling the Microsoft Graph

![Slide](./Slides/Part2/Slide53.PNG)
![Slide](./Slides/Part2/Slide54.PNG)
![Slide](./Slides/Part2/Slide55.PNG)
![Slide](./Slides/Part2/Slide56.PNG)
![Slide](./Slides/Part2/Slide57.PNG)
![Slide](./Slides/Part2/Slide58.PNG)
![Slide](./Slides/Part2/Slide59.PNG)
![Slide](./Slides/Part2/Slide60.PNG)
![Slide](./Slides/Part2/Slide61.PNG)
![Slide](./Slides/Part2/Slide62.PNG)
![Slide](./Slides/Part2/Slide63.PNG)
![Slide](./Slides/Part2/Slide64.PNG)

* [Microsoft Graph Explorer](https://bit.ly/GraphExplorer)
* [MS Graph Postman Collection](https://bit.ly/GraphPostman)
* [Azure AD Postman Collection](https://bit.ly/AadPostman)

![Slide](./Slides/Part2/Slide65.PNG)
![Slide](./Slides/Part2/Slide66.PNG)
![Slide](./Slides/Part2/Slide67.PNG)
![Slide](./Slides/Part2/Slide68.PNG)
![Slide](./Slides/Part2/Slide69.PNG)
![Slide](./Slides/Part2/Slide70.PNG)
![Slide](./Slides/Part2/Slide71.PNG)
![Slide](./Slides/Part2/Slide72.PNG)
![Slide](./Slides/Part2/Slide74.PNG)

* [Teams SSO tab calls Graph sample](https://aka.ms/CallGraphTeamsTab-SSO)

![Slide](./Slides/Part2/Slide76.PNG)
![Slide](./Slides/Part2/Slide77.PNG)

* [Teams SPFx tab calls Graph sample](https://aka.ms/CallGraphTeamsTab-SPFx)

![Slide](./Slides/Part2/Slide79.PNG)
![Slide](./Slides/Part2/Slide80.PNG)

* [Teams Pop-up w/MSAL Calls Graph sample](https://aka.ms/CallGraphTeamsTab-MSAL)

![Slide](./Slides/Part2/Slide82.PNG)
![Slide](./Slides/Part2/Slide83.PNG)
![Slide](./Slides/Part2/Slide84.PNG)

* [Teams Bot calls Graph sample](https://aka.ms/CallGraphTeamsBot-AuthDialog)

![Slide](./Slides/Part2/Slide86.PNG)
![Slide](./Slides/Part2/Slide87.PNG)

More links:

* [Calling Graph from Microsoft Teams(4-part article series)](http://aka.ms/CallingGraphFromTeams)

* [OData Reference](https://bit.ly/ODataSpec)
