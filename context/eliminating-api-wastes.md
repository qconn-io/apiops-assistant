# Introduction

## Why is it essential to remove the “wastes”?
The answer: because they don’t bring any value to the customer, and they take away valuable time and resources from the organization. You can produce more value and revenue with the same resources when there is minimal waste.

The goal of Lean is to improve the cycle time. With Lean API Development and APIOps Cycles, it means you can make better APIs in a much shorter time frame.

Here is some background information for people who are more familiar with Lean already. The APIOps Cycles method is a mixture of Kaizen and 6 Sigma methods of Lean. Kaizen is more about culture inclusive to the whole organization. 6 Sigma change and concentrates more on measuring and chafing special experts to manage the improvements. The basic principle of Lean is Deming’s cycle of Plan - Do - Check (or Study) - Act (or Adjust) and continuous improvement. This is how it originated in Japan’s automotive industry after World War II ended. The principal idea is to improve safety, quality, and speed while reducing complexity. One adaption of Lean principles is Eric Ries’ Lean Startup method for developing business. Lean has also made its way to Lean marketing, Lean enterprise architecture, and Lean software development practices.

The purpose of the APIOps Cycles is to include all the relevant people in the process. One major principle is to improve communication and collaboration. The other principle is to only build the APIs and related technical, marketing, and other assets that produce value. Using this method helps reduce waste in the whole process. It also enables continuous improvement with each step of each Cycle.

Next, we’ll go through the 8 wastes of Lean and see how they manifest themselves in API development. These were important considerations when the APIOps Cycles method was being developed. Organizations could use methods like 6 Sigma or Kaizen to enable them to find out any issues and the potential for any improvements to be made. These or rather other API-specific methods are often needed to improve existing APIs and API teams. With APIOps Cycles, we introduce a ready-made framework for a process as well as tools that will help you start developing APIs. It can significantly help a new team get started but it also works for improving existing APIs. You will still need to make some effort on a case-by-case basis with any new team to adapt it to fit your requirements. Remember to at least make sure everyone knows enough of the method to make full use of it. We do want to make it relatively easy for you to get started. Read the tips in each chapter and consider attending an APIOps Cycles learning program to become a certified user of this method.

## What are the 8 wastes?
There are various names for the 8 wastes, but the core of them stays the same. Originally there were only 7 wastes. We added skills or employee-related wastes to them later. Our favorite list is where the names spell the word **DOWNTIME**; it clarifies why removing waste is essential.

In this e-book, we use this list for the 8 wastes:
1. Defects
2. Overproduction
3. Waiting
4. Non-value-added processing
5. Transportation (or Touches)
6. Inventory
7. Motion
8. Employee and skills waste

Once you have identified the waste sources, you need to figure out what to do with them. Your options are to eliminate the waste, simplify or streamline the process, and minimize producing more waste in the future.

---

## Meet the APIOps Cycle
Great APIs are born when skilled people work collaboratively using a great method. Jump-start implementing APIs by picking up any of the eight phases mentioned below. The full method is available at [https://www.apiopscycles.com](https://www.apiopscycles.com) and is licensed under CC-BY-SA 4.0 Creative Commons license allowing commercial use. Paid support, training, and partnership options are available, too.

1. **Business model**  
   Use API Canvases. Find the right value proposition for your API. Define impact to the business model.

2. **Follow the Minimum Viable API Architecture process.**

3. **Build APIs**  
   Prototype, build, or scale depending on what architecture phase you are currently on.

4. **Audit your API**  
   Use the checklists to verify your API meets style, API management, and security needs.

5. **Publish the API.**

6. **Be mindful of developers’ experience**  
   Support and build a developer community.

7. **Measure business and technical KPIs**  
   Reach your goals.

8. **Learn from the results and improve your API and the process**  
   Or learn the method for the first time.

---

## 1. Defects
Do you know how API is working? Are you missing some information? Is there non-standard processing?

The prominent place to find defects in API development is to look at how the API is working. For example, an invoice handling API might produce the wrong numbers on an invoice. The developers may be using incomplete or incorrect developer documentation.

A defect can also be missing information: an endpoint that doesn’t exist at all; a missing attribute; developers’ documentation that exists only in their dreams; or even an essential requirement for the business logic of the API has not been discovered yet.

These defects can cause a significant amount of rework as well as being very time-consuming and expensive. The more expensive it gets when the problem is noticed late in the development, or the API has published already. Sometimes we see situations where business opportunities are lost because of these defects. And who can afford to lose valuable business opportunities? API providers may need lots of support hours to be able to deal with an incorrect or poorly documented API.

Recently, we were about to use an API that had been working completely fine before. Now, the account balance functionality was broken. Meaning that the whole API was useless because it was a telephony API that consumed balance with every call and SMS. The result: we had to pick a competitor’s API instead.

Non-standard processing can also be considered as a source of defects. That should be obvious but unfortunately it isn’t. There are lots of REST APIs that misuse the HTTP methods described in RFC standards. Sometimes the API providers invent data models of their own even if a standard one exists. Over 50% of the APIs we see on a weekly basis are not using the most common HTTP status codes, or not in a way that they are intended for. Authentication is one of the areas where non-standard solutions thrive. This causes real headaches for developers, or worse still, security issues. Security and privacy should be followed and monitored very closely indeed. Still, we still see big leakages from companies like Google, Facebook, and others. These are due to the design’s failing the stringent privacy requirements. The result: the companies need to shut down those APIs, which others are relying on.

These non-standard design mistakes are very hard or costly to fix when the API is already in production. If they are not fixed, the cost is felt by the developers trying to learn to consume the API or on the lost business opportunities. Non-standard solutions make it very difficult to use an API with standard tooling or API management solutions. The result: the non-standard design may be a complete showstopper.

**Some ways to improve using APIOps Cycles:**
- Collect requirements, as well as relevant standards with the corresponding templates.
- Build only a prototype first.
- Conduct an API consumer interview.
- Use the REST API design guide.
- Use the API audit to validate the design.
- Publish the prototype and make a mock implementation to use for testing purposes.
- Set up metrics that expose potential errors during processing but also bug reports.

---

## 2. Overproduction
API is made bigger, with more endpoints or attributes than needed. Developers are drowning under a massive amount of unnecessary documentation.

Signs of overproduction in APIs are very common. The API is made bigger, with more endpoints or more attributes than it actually needs. The most common overproduction is drowning developers under a massive amount of documentation that is not useful or helpful. Instead, API providers should concentrate on the exact questions and needs that the developers have. APIs and documentation can be extended over time. In many projects and training sessions, it has been observed that 50–70% of first assumptions made by API providers on what their APIs should do are wrong. That’s a big percentage of wrong assumptions. Overproduction causes the API development to take longer than necessary as well as getting the API into the consumers’ hands and creating the expected value.

**Some ways to remove waste caused by overproduction using APIOps Cycles:**
- Use API Canvas to understand the API consumers’ needs and values and what features you want to provide for them to meet those needs.
- Use API Business Model Canvas to get the cost vs. revenue/value metrics with the API consumer segments and the list of things you need to implement to provide the expected value.
- As a minimum, do API consumer interviews to validate your assumptions. It’s better to be safe than sorry – in the long run.

---

## 3. Waiting
Waiting is the waste of time for API developers and API consumers. Waiting for the API or new feature to exist is waste. Waiting for a slow, underperforming API is also waste.

In the full life cycles of an API, there are many times where waiting happens and this waiting can quite easily be eliminated. For instance:
- Waiting for requirements from the business
- Waiting for testers or developers
- Waiting for API keys as an API consumer and not being able to try the API
- Waiting for API documentation while the API is under development
- Waiting for answers to support questions while trying to use the API
- Waiting for sandbox or production environment

Why is waiting time such a waste? Because it’s unproductive, of course. The API developers need to wait for requirements all the time and testing takes ages. The momentum is lost, which creates frustration in the team. It’s totally not helpful for the whole process.

API consumers who need to wait to get access to API keys, documentation, or support will try another API. Internal consumers will find other solutions. These kinds of issues are not good for the business or the health of the architecture.

The APIOps Cycles method promotes collaboration between all the parties involved. They often speak a different “language.” This is achieved using the canvases and other tools provided by the method. The purpose is to concentrate only on the essentials. Only continue to the next stage of the cycles when you have verified the previous one. It minimizes the waiting time caused by questions and reworks. After completing the cycle, all the critical questions for support, marketing, sales, business, privacy, security, testing, and software development should have been answered. You will have a solid starting point at the beginning of the API development process. Everyone can contribute through their work and support developers while the API is being developed. The Minimum Viable API Architecture phase also eliminates waiting from the future API consumers. They can give feedback and start their work weeks or even months before the API version is actually published.

---

## 4. Non-value-added processing
Examples are complex procedures and processes, heavy architecture, project management processes to control API development instead of product management and lean processes, as well as hierarchical process for publishing APIs.

Sometimes it’s not the quantity but the quality that is excessive. Producing “over quality” is called over-processing. Don’t create APIs that are too secure or have all the bells and whistles in the design where less would do. Investing in scalability when you have no idea of the number of potential API consumers is over-processing and it is something you should avoid.

Complex procedures and processes are a form of non-value-added or extra processing. For instance, requiring API consumers to fill in complex forms before getting access to an API can be one example. Having a hierarchical process for publishing APIs is also a form of extra processing. Heavy architecture and project management processes to control API development are termed as extra processing as well.

---

## 5. Transportation (or Touches)
Technical and business people don’t speak the same language: OR too many people involved OR too many separate API requests needed to perform a task.

If you are a developer or technical person reading this, you may think about the actual cost of data that is moved in and out of the API as waste. Uploaded and downloaded data on the internet or with cloud platforms can take a lot of bandwidth. If an application must make many calls to the API to get a simple thing done, it’s considered “chatty.” In that case, the waste is seen because the end-user needs to wait a long time—this is something you don’t want to happen. The waste is the processing time and power to combine the data the application needs to show the result to the end-user.

Let’s put the technical implementation aside. There are other types of transport waste with APIs. Let’s say a business needs a solution with specific data or functionality. They may find an existing API or company that can potentially have an API for that very purpose. Often, the API documentation is written in a language that doesn’t mean a thing to a non-technical person. This means there needs to be more people involved on the customer side and possibly the vendors’ side, too. Sometimes when buying a fit-for-purpose API, the provider insists on having a demo. After a 30-minute session of “How,” “Why,” and “What” to show you how to use the API, you finally get your hands on it. Then comes signed contracts by CXOs and a heavy onboarding process.

In one case alone, starting to use an API involved four persons on the vendor’s side and five persons on the buyer’s side. Looking at the monthly cost of the API, this wasn’t justifiable. Unfortunately, this is not an isolated case either. Many API providers work like this to the detriment of their businesses.

Fixing these problems by using the APIOps Cycles method requires using:
- The API Business Model canvas to define the channels and methods of handling the customers’ relationship for the API and doing profitability calculations
- The API Consumer interview
- The Network and systems requirements template when collecting
- The Developer experience checklist

---

## 6. Inventory
Creating APIs that are not immediately used by API consumers is inventory waste.

Creating APIs that API consumers do not immediately use is inventory waste. Creating a backlog full of requirements even though 10% could be implemented in the next development cycles is a total waste. The conditions may change rapidly and an element of (re)organizing and (re)prioritizing may need to take place—even several times depending on the specific circumstances. Scaling the architecture before there’s not so much traffic for the API is also a waste.

One example of this was a large organization wanting to start an API program and purchase an API management platform. They didn’t have any APIs at that moment in time. They also didn’t have any knowledge of internal or external needs that would require APIs. The IT department still wanted to go ahead and build their first API. One of the projects that they were starting could perhaps use this API. They didn’t want to disclose to anyone they had begun making APIs before they had their first API operationally ready. They re-booted the process using the APIOps Cycles method. Then they discovered something interesting. Their first API was estimated to cost more than it would bring in cost savings, additional revenue, or any other value in 3–5 years. Their plans had to change. They continued with their original plans but with a much-reduced scope. They now paid more attention to interviewing future API consumers’ needs, so that they could build an API more tailored for their consumers’ needs and requirements as well as be user-friendly.

---

## 7. Motion
Waste from an individual efficiency point of view.

Motion is a waste from an individual efficiency point of view. Imagine you are cooking in a kitchen. You need water, a fridge, utensils, etc., to be close by so you don’t need to move around the kitchen all the time when preparing food.

During API development, businesspeople, architects, and other parties should be able to discuss their requirements. It should be a quick process, happening across only a few meetings, and with minimal paper pushing as possible. Business owners, product managers, and support need to contribute to API documentation without disturbing the ever-busy developers. Clear boundaries should be set for the process.

With APIs, motion can be viewed from two perspectives: the API consumer’s or the API providers’ point of view. Good developer experiences happen when the API-consuming developer can start using the API with his favorite tools with just a few clicks and has all the relevant documentation at hand. If the API consumer is a non-developer and wants to use the API with his favorite integration platform, that should be possible to do with only a few clicks and with the least effort, too.

From the API provider’s point of view, the development and deployment of code, interface, and documentation should be super easy. Developers don’t want to use API management tools or write documentation. They just want to type “commit,” and everything gets added to version control, tested, deployed, and published. This is where APIOps gets close to DevOps.

APIOps tries to eliminate Motion waste by giving design guidelines, audit lists, and processes that promote automation throughout the process coupled with a suitable API management solution and standard interfaces.

---

## 8. Employee and skills waste
An untrained and unmotivated API team is not cost-effective. APIs that require developers to study hard before understanding the API.

Creating APIs with processes unfit for API development is a waste. Underutilizing people’s talents can also be a form of waste, too.

Not involving future API consumers, marketing customer support, businesspeople, privacy, API management tool specialists, and many other experts in API development may seem like a cost-effective thing to do at the time. It can cause problems later on when these people need to be able to understand, publish, support, sell or otherwise contribute to the API lifecycle. Wasting time translating technical API terminology or understanding business jargon can be included as a waste here, too. Effective cross-silo collaboration and communication doesn’t just happen; they need to be planned—with precision.

Not training the API team properly can also bring its own set of unique problems. They are either idle or unproductive, or product designs and implementations that don’t meet the set requirements and standards are produced. Often the problem is not that the developers can’t program, it’s just that they don't know how to design and implement APIs that can fully meet the required standards. The most challenging part of the process is to be able to meet the API consumers’ needs or have a good developers’ experience from onboarding to using the API. More skills are needed than just software development to make effective developers’ journeys a reality.

Research shows that the best APIs thrive where marketing and developers co-exist. Employee waste can also be caused by overqualified people doing work that they are not motivated to do. This often happens when API development is not appreciated and is reduced to just the basic implementations. Sometimes good people drown under masses of bug reports, support questions, and other non-development-related work. This is usually caused by not using continuous integration, automated testing, and metrics. Also, not including documentation in the same pipeline is just asking for trouble. So, try to avoid all of these from occurring.
