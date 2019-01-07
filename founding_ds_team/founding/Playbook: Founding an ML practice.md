# Playbook: Founding an ML practice

tl;dr: TODO

As part of his company's transformation to a technology company, Capital One's founder and CEO Rich Fairbank 
identified the need to found a Machine Learning center of excellence. I was very fortunate to co-found that center of
 excellence, and I've learned a few things from the experience.

## Opportunity

I won't beat around the bush: Data Science is ["The Sexiest Job of the 21st Century"](https://hbr
.org/2012/10/data-scientist-the-sexiest-job-of-the-21st-century). Perhaps more importantly, bringing on Data 
Scientists is also one of the most valuable investments a company can make. 

No one wants to be Blockbuster; and no one wants to be left in the dust of the data revolution. This is why leaders 
like AirBnB, Facebook and Google are hiring data scientists at breakneck speeds, and Data Scientists to every 
engineering team. 

These hires aren't for vanity; machine learning is [transforming corporate America](http://fortune
.com/ai-artificial-intelligence-deep-machine-learning/), with highly visible wins including AI assistants, driver-less
 cars, and machine translation leading the way for less visible wins (like 
 [authorization fraud](https://stripe.com/us/radar) and [AirBnB's search](https://medium.com/airbnb-engineering/applying-deep-learning-to-airbnb-search-7ebd7230891f))

## Steps

TODO intro 

### Get support

Some company leaders will just get it, and others might see the risk of falling behind the industry. However, it 
still might be helpful to find a case study of a similar company that's profiting from their Data Science team, or 
new products in your industry that are centered around Data Science. Even better, a brief proof-of-concept project 
could help highlight the low-hanging fruit you and your team could tackle.  

Once you've got support and buy-in from your leadership, you can begin a backlog of projects that data science would 
enable, and how your data science team will integrate with existing software engineering and data engineering 
resources. Even if your existing team and leadership don't have quite the right way to phrase their pain points and 
ideas as data science problems, this backlog will help prioritize hiring and first team projects. 

### Hire

Now that we have support and potential projects, you can start hiring. We'll cover hiring in-depth in a future blog 
post, but this might be the most difficult part of the journey: Data Scientists are greatly in demand. Moreover, 
those with experience forging a team likely know their market value, and can afford to be picky. 

To get candidates in the funnel, I'd recommend generating organic leads through Meetup groups and conferences 
(but really conference receptions). Sources and hiring agencies can be worth while, but form emails are easy to 
ignore in a hot market. A quick survey of DS friends suggest we receive an average of 30 recruiter messages a week, 
and it's hard to stand out in that chaos.   

It'd be wise to choose a first few hires with proven track records of building products, and / or mentoring others. 
As the team grows, there may be room for R&D and specialized roles, but early on it'll be all hands on deck proving 
value.

If you happen to have existing software engineers or data engineers with a math background (or a good amount of grit)
, it may make sense to provide them with time and training to skill-up into a Data Science role. Existing team 
members know the company & culture already. Also, providing a skill-up opportunity can help with retention and 
keeping your A-team up-to-date and mentally challenged.   

### Form team

Once you've got your motley crew together, it's important to build a strong foundation for your forming team. 

Data Scientists uniquely come from a variety of backgrounds and practices, and might come to the table with a (wide) 
diversity of skills, work flows and preferred tools. Have conversations early and often about best practices, and 
what team members can expect from each other. If you subscribe to the Agile or Scrum dogmas, now's the time to 
indoctrinate. 

Nothing forms a team quite like a shared crucible: If there's a particularly high-value, low-effort project in your 
backlog, this will help your team learn how to work together while gaining everyone some visibility within the 
company. Otherwise, data engineering and data lake projects could enable many more Data Science projects, and help 
your team get familiar with their new data. 

After you get your footing with your first few projects, begin talking about what your standard workflow looks like, 
libraries and infrastructure you'd like to build, and the cost of technical debt.

I'd also recommend scheduling monthly happy hours or other fun events. It's important for teammates to trust each 
other, and get to know each other out of the office. Also, your new hires are probably getting recruiter calls 
already, and beers are less expensive recruiting. 

### Bring value

Alright, now we've got a strong team of Data Scientists, who've proven themselves with some minor projects. On this 
foundation, you can start earning the support and buy-in your leadership has invested in you. 

Though you might have done a few initial projects, your first major project will help to define your team, and your 
team's role within the company. Choose a major project that can be done in milestones, provides a high visibility 
win, and that you know you can deliver on. Great first projects include creating a new data warehouse, creating a 
homegrown alternative to a vendor model, or creating a viable new product offering. 

Once you're about 60% done with your first project, start presenting to other groups to get their feedback and buy-in
 (and shake out any new project proposals). At about 80% done, you could start presenting the project up the food 
 chain, to help leadership understand how their investment is paying off. 

Once your first project is over, just keep pumping them out!

## Lessons learned

Before you go and conquer the world, there are a few last lessons learned that might be helpful: 

### Augment, not replace

It's easy to fear being replaced by the machines. Before calling the old staff luddites, help them to realize that 
in general, your team will augment and streamline their role, rather than replace it. Most of my data science 
projects have alleviated the boring part of other's roles, and allowed them to leverage their specialized 
skill sets. For example, a recent project allowed lawyers to spend less time sorting mail, and more time practicing 
law. Another great case study was security analysts to spend more time evaluating trends, and less time scrolling 
through email logs. 

### Tribal knowledge

While Data Science is the hot new skillset, there's still a lot of value in the domain (tribal) knowledge your 
company has built up. Whether it's knowing that `cdt` really means `charge_off_date`, or that the company's proxy 
requires voodoo witchcraft to work, there's a lot that the existing staff can teach your new team. Embrace this help,
 don't fight it.  

### Embedded vs monolith

One of the largest ongoing discussions in the Data Science (other than 
[tabs vs. spaces](https://www.businessinsider.com/tabs-vs-spaces-from-silicon-valley-2016-5)) is whether data science
teams should be embedded (with data scientists on each product team) or monolithic (with all data scientists on one
team). Embedded data science teams allow data scientists to build product knowledge and specialization, and the data 
scientists' goals aligned with product goals. Monolithic data science teams make standardized workflows and 
skillsets, provide Data Scientists with a brain trust of peers. 

A popular approach get's the best of both worlds by hiring Data Scientists into a Data Science 'guild', providing 
regular Data Science guild meetings, and deploying Data Scientists to different product teams. 

### Project planning

The most common misconception I've seen is running Data Science teams like Software Engineering teams. While there is
 a lot of overlap, generally software teams are able to define their features and milestones at the start of a 
 project. Data Science projects tend to be less linear, with scope evolving as data quality, research, and model 
 training inform future iterations.  

## Go forth, and conquer

Now that you've got your playbook, go forth and get some buy-in. Data Science is rapidly transforming corporate 
America, and no one wants to be left in the dust. 
