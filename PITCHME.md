---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Bringing your ideas to life quickly and cheaply
![](https://blog.ironmoosedevelopment.com/content/images/2018/12/moose-head-harvest-small.png)

https://github.com/IronMooseDevelopment/awesome-cheap-tiers

Note:

- You probably have an idea you would like to work on
- You'll learn what resources and tools are available to you to make that idea happen
- You'll learn how to make your idea survive the Reddit hug of death without breaking the bank


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

## Who am I?

Note:

- CEO & Founder of Iron Moose
- Developer for over 11 years, professionally for 6
- C#, NLP, Bots, Automation, Active member of open source
- We run our company on less than $25 / month and have a product
- Gonna talk about the challenges we faced and lessons we learned when trying to build an always-up product (scale + maintainability)
- Humblebundlebot


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

## Why build quick and cheap?

Note:

- Three resources: Time, Money, Energy
- There are only 24 hours in a day and a person has limited energy to work on something
- Energy vs Time - something can be easy but take forever (manually editting 1k files) vs hard but take little time (scripting it)
- Big companies can scale up energy by hiring more people but there's still only 24 hours in a day so they favor spending money to reduce total time needed
- Side projects have infinite time - you have no due date - but limited funds and energy
- "Quick" focuses less on calendar time and more on energy needed to complete something



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

## Why build auto-scalable?

Note:

- A majority of the time your service will go unused (sleeping, low user counts, daily jobs)
- Scaling down to 0 saves money
- A sudden surge of traffic (Reddit viral) will overload a cheap server
- Scaling up to Infinite lets your service survive
- Letting service providers scale up / down your code for you based on demand is called "serverless"
- Virality is the cheapest marketing
- Scalability indicator


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

## Planning

Measure twice, build once, deploy continuously

Note:

- Why does it matter?
- First step on any journey
- Most things die at this stage or get forgotten

---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Organizing Ideas and Work

You have ideas, write them down

Note:

- Kanban vs Sprint
- Sprints are good when you have a product owner / client you need to show steady progress to OR if you can commit to a release at the end of every sprint and have predictable hours
- Kanban is good when you just have a pile of work to steadily work through and varied hours-per-week



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-45 text-center text-black]
![Azure Boards](images/azure_boards_logo.png)
@size[.7em](@fa[quote-left](A scrum / kanban board that comes as part of Azure Devops))

@box[bg-purple text-white](Free#Up to 5 Developers, unlimited Stakeholders)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://azurecomcdn.azureedge.net/mediahandler/acomblog/media/Default/blog/0059bc84-b75f-4129-b09b-dd1a64944a9e.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Trello#Free - 1 Power-Up, 10MB max, 10 team boards)
@box[bg-blue text-white text-05](Github Project Boards#Free - Up to 3 developers for private repo)
@snapend

Note:

- We take advantage of unlimited stakeholders to arrange ideas and non-development work
- Configurable, we add "Tech debt", "research", and "blog posts" as item types

+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-45 text-center text-black]
![0nenote](https://i0.wp.com/mykidslocker.com/wp-content/uploads/2016/01/Screen-Shot-2016-01-17-at-8.54.11-PM.png?resize=150%2C150)
@size[.7em](@fa[quote-left](Microsoft's notekeeping app, part of Office))

@box[bg-purple text-white](Free#Up to 5 GB)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://www.onenotegem.com/uploads/8/5/1/8/8518752/main_2_orig.jpg)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Evernote#Free - Unlimited notes, no team features)

@snapend

Note:

- File doesn't need to be saved - persists through restarts for you


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Team Chat

Hurray for collaboration!

Note:

- IM, VC, Screen Share, File Sharing




+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Discord](https://img.wennermedia.com/article-leads-horizontal/discord-logo-685bbc5f-8221-4a45-b809-4dc5e38c22fc.png)
@size[.5em](@fa[quote-left](An IM option aimed at gamers, Discord offers excellent channel organization options with no limits to voice channels, screen sharing, or message history.))

@box[bg-purple text-white](Free#8MB File Upload, 720p screen share)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://proxy.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn-images-1.medium.com%2Fmax%2F1600%2F1*W3JjjfzTJOL9V9TvDU1MFA.gif&f=1)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Slack#Free - 10k Message history, 10 apps, no group calls)
@box[bg-blue text-white text-05](Microsoft Teams#Free - 100 Users, 2GB storage / user, no 2FA)

@snapend

Note:

- Organization & Pinning resources helps fuel discoverability
- Unlimited history is important for decision making
- We already all had Discord for gaming, so people are logged in far more often and see messages

---?color=linear-gradient(to top, #f3ab40, #f0d57d)

## Building

Make sure you have the right tools for the job

---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Code Repos

Because CTRL-S isn't quite enough at times






+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
#### Azure Repos
![Azure Repos](https://ms-vsts.gallerycdn.vsassets.io/extensions/ms-vsts/team/1.149.2/1551279954328/Microsoft.VisualStudio.Services.Icons.Default)
@size[.5em](@fa[quote-left](A Git repo that comes as part of Azure Devops))

@box[bg-purple text-white](Free#@size[.7em](Unlimited public and private repos, up to 5 developers))

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://www.dotnetcurry.com/images/devops/vsts-azure-devops/azure-repos.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Github#Free - Unlimited public and private repos, up to 3 developers)
@box[bg-blue text-white text-05](Gitlab#Free - Unlimited private repos and developers, no merge approvals)

@snapend

Note:

- Auto-merge pr when build passes
- Integrates well - can track work across the entire stack
- Well-built code viewer with essentially visual studio code



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Frameworks

Baking bread is a lot faster with premade dough



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

![](https://prnewswire2-a.akamaihd.net/p/1893751/sp/189375100/thumbnail/entry_id/0_w5dofghs/def_height/400/def_width/400/version/100012/type/1)

Open source C# framework for apps that compiles to native Android, iOS, Mac, and UWP with maximal codesharing

![](https://www.technovert.com/wp-content/uploads/Xamarin-1.png)


Note:

- Android, android auto, iOS, Mac Desktop, Windows Desktop, Xbox, Hololens, smart watches, smart tv's
- Would support Linux if they could agree on a standard Window api
- Experimental support for webassembly

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Blazor

Open source C# framework for websites that compiles to webassembly

![](https://learn-blazor.com/images/getting-started/blazor-architecture.jpg)

---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Authentication

It's hard and necessary

Note:

- OAuth and why it's nice
- Why you should offer user-password logins as well
- Security is *hard*





+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Auth0](https://images.ctfassets.net/2ntc334xpx65/40dfJ4MoDmkkOuO2qakkGG/34f994d35925dd81be615e82a2544b3d/Logo_2x.png)
@size[.5em](@fa[quote-left](Wraps OAuth options into one management layer for easy integration.))

@box[bg-purple text-white](Free#7000 active users, 2 social providers)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](http://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2016/02/1454698917angular-auth-1.png)
@snapend


Note:

- Manages social & username-password logins for you, and allows customization with serverless rules



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Databases

Store data. Serve it back up later. Don't leave this with default credentials.

Note:

- A few types of DBs
- Schema-based (SQL)
- Schema-less (noSQL, Document DB, Key-Value DB)
- Schema-less is faster for development but harder to optimize for performance
- There's plenty of performant production instances of no-sql, it just takes a different approach to data modeling - one size does not fit all!





+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Azure Table Storage](https://datadog-docs.imgix.net/images/integrations_logos/azure_storage-7ee8b362.png)
@size[.5em](@fa[quote-left](A Key-Value database that scales automatically and stores your data globally))

@box[bg-purple text-white]($0.045 / GB / Month#No Limits))

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://sec.ch9.ms/ch9/fb08/bffcf8dc-f626-4bc0-aaf8-c1853c59fb08/CustomizeTableColumnsInMicrosoftAzureStorageExplo_960.jpg)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Azure Blob Storage#@size[.7em]($0.0184 / GB / Month, various read / write prices - Prices increase after 50 TB / month))
@box[bg-blue text-white text-05](mLab#Free - 0.5 GB storage)

@snapend

Note:

- Various replication options offer increased global speeds for increased costs
- Azure Serverless SQL exists



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Email

Still a great way to reach people

Note:

- Transactional is based on user actions - signing up, buying an item, getting an invite to a new group, etc
- Marketing is based on a mail list - All signed up users get your weekly newsletters, etc
- It's surprisingly hard to keep these two kinds of email in sync with each other



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Sendgrid](https://sendgrid.com/wp-content/uploads/2016/06/SG_Logo_Blog.jpg)
@size[.5em](@fa[quote-left](Transactional email API with good library support and a matching Marketing email offering))

@box[bg-purple text-white](Free#100 emails / day)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://www.ventureharbour.com/wp-content/uploads/2014/04/sendgrid-analytics.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Mailgun#Free - Transactional email API with an email validation sister API)

@snapend


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Graphics and UX

The best app in the world is useless if no one can interact with it



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Fiver](http://thetravelingdutchman.com/wp-content/upload_folders/thetravelingdutchman.com/2016/03/Fiverr.jpg)
@size[.5em](@fa[quote-left](An online marketplace of freelancers providing various services such as graphical and UX design))

@box[bg-purple text-white]($5 and up / design#No Limits)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[east span-50]
![](https://cdn.lifehack.org/wp-content/uploads/2014/01/fiverr-1024x526.png)
@snapend

Note:

- We've got most of our graphics done through a single guy Noko
- After initial back and fourth he was able to turn our ideas into excellent reality quickly
- Loyalty helps get good results



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Figma](https://i0.wp.com/wptavern.com/wp-content/uploads/2018/11/Screen-Shot-2018-11-19-at-8.43.27-PM.png?ssl=1)
@size[.5em](@fa[quote-left](A browser-based UX tool with easy collaboration and code-exporting for styles))

@box[bg-purple text-white](Free#2 team members, 3 projects, 30 days version history)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[east span-50]
![](http://www.bestetools.com/wp-content/uploads/2018/03/FIGMA.png)
@snapend



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Documentation

Answer your user's questions ahead of time instead of at 3am




+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
### Github Wikis
@size[.5em](@fa[quote-left](Markdown wiki hosted by Github and included with every Github repo))

@box[bg-purple text-white](Free#3 Developers per private repo)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://raw.githubusercontent.com/bitmovin/github_wiki_index/master/index.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Read the Docs#Free - Open Source projects only, no private documentation, ad supported)
@box[bg-blue text-white text-05](GitBook#Free - 2 Users, 1 Public space, 1 Private space)

@snapend


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Metrics and Logging

If debugging is an art, then Metrics and Logs are your paintbrushes

Note:

- Metrics are counts of how many times something happened
- Logs are details of what happened and why
- Logs can either be single-line "tail" logs or json-based "structured" logs

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-45 text-center]
#### Azure Application Insights
![](https://docs.microsoft.com/en-us/azure/application-insights/media/app-insights-dashboards/010-oview.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](An end-to-end sampled view of user interactions that can be installed in one-click for most Azure resources))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#5GB storage / month, 90 days retention)
@snapend

Note:

- Includes Metrics
- We use this to keep a pulse on how performant our services are and where users are getting stuck


+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-45 text-center]
#### Papertrail
![](https://papertrail.global.ssl.fastly.net/images/screenshots/search.png?1528999755)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Solarwinds provided aggregated tail logs with automatic filters for non-structured logs))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#50MB / month, 7 days retention)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-45 text-center]
#### Loggly
![](https://d2gn4xht817m0g.cloudfront.net/p/product_screenshots/images/original/000/492/684/492684-e939f89cc34a8b144279d933c3db862ab3f9def6.png?1426716161)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Solarwinds provided aggregated structured logs with filters))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#200MB / day, 7 days retention, no alerts)
@snapend



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### CI / CD

Building and deploying code is for bots, not humans

Note:

- Hosted agents are managed by the service and usually don't cache dependencies
- Self-hosted agents are managed by you but have performance and privacy gains



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Azure Pipelines](https://chrisjarrintaylor.files.wordpress.com/2019/02/azure-pipelines.png?w=712)
@size[.5em](@fa[quote-left](A CI / CD chain that comes as part of Azure Devops))

@box[bg-purple text-white](Free#@size[.5em](1 Hosted agent @ 1800 build minutes / month, 1 Self-Hosted agent))

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](http://ilikesqldata.com/wp-content/uploads/2018/09/azurecomcdn.azureedge.net7785b324-37ed-4035-981f-e-b6349c425c24c9fb7fd9ee3736d6ff807dc76c73.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Bitbucket Pipelines#Free - 50 build minutes / month)

@snapend

Note:

- Flexible templated CI / CD

---?color=linear-gradient(to top, #f3ab40, #f0d57d)


### SaaS

Other things that might help you along your way

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
#### Azure Search
![](https://www.microsoft.com/developerblog/wp-content/uploads/2016-12-10-Azure-Search-QNA/19.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](AI-Powered search index that integrates easily with SQL and Azure Table Stoarge))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#50 MB, 3 indexes)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
#### Azure Playfab
![](https://playfab.com/assets/img/add-ons/xsolla/xsolla-hero.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Multiplayer game services in a box, incuding profiles, commerce, and leaderboards))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#No professional features)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
#### Microsoft Flow
![](https://mspoweruser.com/wp-content/uploads/2018/12/Microsoft-Flow-Beta-696x434.jpg)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](A code-free logic flow creator that connects to popular sources))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#No Limits)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-45 text-center]
![Moosetracks](https://moosetracks.app/assets/img/moosetracksslim.png)
![](https://i.imgur.com/qXwAOaa.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.4em](API debugger by Iron Moose Development that collects API calls from your app / service for easy visualization and built-in issue analysis))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#1k requests / month)
@snapend


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

## Hosting

Because you can't show people your cool project on your laptop forever

---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### IaaS

Full environments where you have near-complete control



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Digital Ocean](https://venturebeat.com/wp-content/uploads/2017/06/digitalocean-logo.png?fit=1100%2C854&strip=all)
@size[.5em](@fa[quote-left](Developer-focused VM provider with easy DNS setup and one-click-deploy options))

@box[bg-purple text-white]($5 / Month#1GB RAM, 25GB SSD)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://puppet.com/docs/pipelines-for-apps/free/images/NodeTutorial/digitalOceanSetUp.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Azure Linux VMs#$0.0075 / hr - 1GB RAM)
@box[bg-blue text-white text-05](Azure Windows VMs#$0.008 / hr - 1GB RAM)

@snapend

Note:

- Azure VMs can temporarily burst to handle higher loads



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### PaaS

Takes the underlying OS out of the equation so you can just focus on your App

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
### Azure App Service (Free)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[red](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Host your site / service straight out of Visual Studio for free on shared infrastructure))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#1GB RAM, 1GB Storage, 60 minutes / day)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
### Azure App Service (Shared)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[red](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Host your site / service straight out of Visual Studio for free on shared infrastructure))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#$0.013 / hr)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#1GB RAM, 1GB Storage, 240 minutes / day)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
### Azure App Service (Basic)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Host your site / service straight out of Visual Studio for free on shared infrastructure))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#$0.075 / hr)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#1.75GB RAM, 10GB Storage)
@snapend

Note:

- First tier that offers auto-scale features based on configurable criteria: not quite full serverless however

---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### FaaS

Takes the underlying App out of the equation so you can just focus on your functionality



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Azure Functions](http://taswar.zeytinsoft.com/wp-content/uploads/2017/12/MSAzure-functions.png)
@size[.5em](@fa[quote-left](Azure hosted functions that spin up on the fly based on triggers))

@box[bg-purple text-white](Free#@size[.7em](1 million executions))

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://proxy.duckduckgo.com/iu/?u=https%3A%2F%2Fimage.slidesharecdn.com%2Fintrotoazurefunctions-160504044340%2F95%2Fintroduction-to-azure-functions-tutorial-5-638.jpg%3Fcb%3D1470734076&f=1)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Iron Functions#Self-Hosted)

@snapend

Note:

- GBs = MB of RAM * CPU run time seconds


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Static Sites

Advertise your service and explain how to use it




+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Github Pages](http://www.recursosweb.es/wp-content/uploads/2014/04/github-pages.jpg)
@size[.5em](@fa[quote-left](A Github hosted static site solution - just push and host. Great for project readmes))

@box[bg-purple text-white](Free#@size[.7em](1 per Account / Org, 1 per Project, Non-Commercial))

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://pages.github.com/images/choose-layout@2x.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Netlify#Free - 1 Developer, 1 Concurrent Build)
@box[bg-blue text-white text-05](Azure Storage Static Site#Free except Azure Storage Pricing - No Limits)

@snapend



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

## Scaling Up

For when you have more than 10 users

---?color=linear-gradient(to top, #f3ab40, #f0d57d)


### Status Pages

Let people know you are down so they come back when you are up




+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Cachet](https://proxy.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.brandeps.com%2Flogo-download%2FC%2FCachet-01.png&f=1)
@size[.5em](@fa[quote-left](Open source Status page with multi-language and planned downtime features))

@box[bg-purple text-white](Self-Hosted#No Limits)

@snapend

@snap[south-west span-20]
@size[1.5em](@color[red](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://blog.5apps.com/images/screenshot-cachet.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Freshstatus#Free - Up to 250 subscribers, no scheduled reports)

@snapend



---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Marketing

Let people know you exist



+++?color=linear-gradient(85deg, #f2f2e2 50%, #f3ab40 50%)

@snap[west span-40 text-center text-black]
![Mailchimp](https://proxy.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.stickpng.com%2Fassets%2Fimages%2F58417f77a6515b1e0ad75a2c.png&f=1)
@size[.5em](@fa[quote-left](Marketing email platform with easy email designer and landing page creator))

@box[bg-purple text-white](Free#@size[.6em](7 channels, basic templates, 2k contacts))

@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
![](https://cdn0.capterra-static.com/screenshots/2073942/44314.png)
@snapend

@snap[south-east span-40 text-center]
#### Alternatives

@box[bg-blue text-white text-05](Sendgrid#Free - 2k contacts, 6k emails / month, 1 user)

@snapend


+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![Ghost](https://www.citycloud.com/wp-content/uploads/2013/10/ghost_logo_big.png)
![](http://2.bp.blogspot.com/-8qYtJKgfCjE/Uk7R400w_wI/AAAAAAAAAws/oXh5Clw5ynU/s1600/ghost-admin.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[red](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](A popular open source publishing platform for blogs and journals))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Self-Hosted)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#No Limits)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
#### Landbot
![](https://wp-handpicked.com/wp-content/uploads/2018/08/landbot.jpg)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](A chatbot bot driven landing page that directs users through to what they want to know))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#100 chats / month, 30 logic blocks, basic integrations)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![GitPitch](https://gitpitch.com/docs/images/logo.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](A git-enabled markdown-powered presentation tool))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#Public repos only, no exporting)
@snapend


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Finances

Pay people money

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![Waveapps](https://www.waveapps.com/sitestatic/public/img/wave-media-logo-2.png)
![](http://fbalibrary.com/wp-content/uploads/2017/06/WaveApps-Featured-1-1.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Invoicing software with a payroll option for both employees and contractors))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#@size[.5em](Free for accounting / invoicing / receipts, $20 / month + $4 / person for payroll))
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#No Limits)
@snapend


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Invoicing and Subscriptions

Get paid

Note:

- Invoices are for active work completed (one time or recurring)
- Subscriptions are passive for work provided

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![Invoicely](https://assets.pcmag.com/media/images/490874-invoicely-logo.jpg?width=810&height=456)
![](https://designshack.net/wp-content/uploads/feature-invoicing.jpg)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Estimate and Invoicing tool designed for the web, hosted by ApiLayer))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#1 User, PayPal only, no Recurring)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![Chargebee](http://www.iamwire.com/wp-content/uploads/2014/01/Chargebee.png)
![](https://cdn0.capterra-static.com/screenshots/2092486/32447.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.4em](Subscriptions-as-a-service offering that allows users to manage their credit cards and subscriptions in a hosted page.))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#First USD $50k revenue)
@snapend


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Support

End-users will always need help

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![](https://www.purechat.com/img/index/pc-whitebg-logo.adec9123.png)
![](https://s17528.pcdn.co/wp-content/uploads/2015/07/Pure-Chat-example-conversation.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Livechat support that falls back to email if no one is online to answer a question))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#Unlimited chat, 3 Users, 1 website)
@snapend


---?color=linear-gradient(to top, #f3ab40, #f0d57d)

### Legal Compliance

The not-fun part that helps you not get sued

Note:

- You should probably form an LLC - $50 through a provider or cheaper through the state gov

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![Termly](https://termly.io/wp-content/themes/genesis-tly-v3/build/images/logo-dark.svg)
![](https://termly.io/wp-content/uploads/2018/11/step01-1060x466.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Automatic generator and hoster of Terms of Conditions and Privacy Policy documents))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#1 Policy)
@snapend



+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![Cookie Consent](https://cookieconsent.osano.com/assets/images/logo__cookie-consent.png)
![](https://cookieconsent.osano.com/app/uploads/2016/07/img__about-cookie-consent-1-1-1024x588.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.5em](Open source Cookie Consent banners provided by Osano))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#No Limits)
@snapend

Note:

- Customizable

+++?color=linear-gradient(to top, #f3ab40, #f0d57d)

@snap[west span-40 text-center]
![Eversign](https://designshack.net/wp-content/uploads/eversign-logo.png)
![](https://smallbiztrends.com/wp-content/uploads/2017/04/eversign-review-850x476.png)
@snapend

@snap[south-west span-20]
@size[1.5em](@color[green](@fa[line-chart]))
@snapend

@snap[north-east span-50]
@box[bg-purple text-white](Summary#@size[.4em](Legally-binding eSignature platform with Google Drive template importing features hosted by ApiLayer))
@snapend

@snap[east span-50]
@box[bg-green text-white](Price#Free)
@snapend

@snap[south-east span-50]
@box[bg-orange text-white](Limits#5 documents / month, 1 user)
@snapend



### In Conclusion
![](https://blog.ironmoosedevelopment.com/content/images/2018/12/moose-head-harvest-small.png)

https://github.com/IronMooseDevelopment/awesome-cheap-tiers

Note:

- You'ved learned what resources and tools are available to you to make your idea and survive the Reddit hug of death without breaking the bank
- No resource can help you if you run out of steam and give up
- Find some friends - it's more fun together