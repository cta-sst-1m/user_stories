# SST1M User Stories

Welcome to the SST1M User Stories. This repository should become a collection of issues. Only issues? No code

Yes, exactly.

We want to collect stories of users (and developers of course) telling other developers what "features" are needed somehow somewhere in the SST1M software collection. 

This is an experiment. So let us think big here, there should be no limit to these stories. You are allowed - yes expected even - to write down any feature that comes to mind. Might be very high level like:

> I want to be able to plot a spectrum, from a bunch of runs. 
  
Or something low level like:
 
> The `run_id` seems to be always zero, I'd like it to be some useful number.
    
We are a bit late with these user stories, so there are already a bunch of feature which work, like:

> I want to be able to calculate the dark baseline from a bunch of run files.
> 
> -> You can, use dark_evaluation.py :-D
    
Still if you realize something is already working, but there is no user story for it, please take a minute to write it down.

# What are these user stories used for?

Software design is a difficult art. Possibilities are limitless and deciding where to stop often a challenge. Without a definition of "goals" designers would sometimes "overshoot". They would create something that has many features and can do great things.

However, features come at a cost. They cost "lines of code". Did you know that code is ten times more often read than written? So unneeded features start costing a lot very quickly.

Also, code tends to rot, features break. This means, some developer creates a useful tool once .. and used it. Then she went on. Some time later a user comes by, spots the tool and tries to use it ... BAAM!! ... exceptions all over the place. Why? Because the tool was allowed to rot. Something was modified somewhere .. the tool depended on it .. nobody used the tool for a while, so it broke.

This means, tools need to be tested. Tests are often forgotten. So some tools might be broken at the moment and nobody knows it. Also some features might be broken and nobody knows it. So in order to find out what the SST1M software should be able to do, we need user stories.

The more the better. 

It is fine, if there is a story for a feature we only need in a year from now. That story can be converted into a plan.
It is fine if there are stories about features, which later turn out to be not needed anymore. Software is dynamic, we can change it.

# The What and the How

A user story should strive to explain what is needed. How to implement it is more a question for the developer who implements it. 

Performance requirements can be included if course. Quantitative requirements are more useful than qualitative requirements, so:

> I want the reader to be fast and not use too much memory.
    
Is a user story, but:

> I want the reader to read 1000 events per second (single thread) from a solid state disk. The memory used per event by the reader should not exceed 10MB. 
    
Might be more useful for developers.

Still, the first version is way way better than no story at all. If a user story is difficult to turn into code, we can ask the author of the story, or discuss it on a telcon or so. 
