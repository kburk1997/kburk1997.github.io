---
layout: post
title:  "CrowdCop - Presentation Complete!"
date:   2016-03-28 15:33:19 -0400
tags: [crowdcop, rcos, django, update, fullstack, python]
comments: true

---
Adapted from: [https://rcos.io/projects/bocaaust/CrowdCop/blog](https://rcos.io/projects/bocaaust/CrowdCop/blog)

Last Tuesday, we did a mock presentation of our project and it was very shaky. The last time we presented, we didn't have much to present, so it was very easy. This time around, we had a lot to cover in so little time, and the reason why our mock presentation was shaky was because we tried to cover everything.

Friday's presentation went very well. We showed off our progress and had a local demo ready. This time around, we did a demo from the user's point of view and not our point of view. That way, we could state <i>what</i> we implemented before demoing, and it gave us a chance to focus on <i>why</i> the average person should use it. Our audience got a good feel for the UI/UX of the product, and this led to a smooth run.

In early March, I had all the templates done and needed to implement the MVC functionality and integrate with the database. I am excited to say that the MVC functionality and database integration are complete for our local test, as well as user authentication features. 

Here's what we still need to work on before we have a finished product to test on campus:

<ul>
<li>Migrate our local test to the web server</li>
<li>Track crowdfunding contributions:</li>
<ul>
<li>Per campaign - that way we can store how much money has been crowdfunded towards a certain campaign</li>
<li>Per user - user's crowdfunded contributions will show up on their profile under "Contributions"
</ul>
<li>Allow a user to "follow" certain campaigns they feel strongly about - these show up under "Following" in the profile</li>
<li>Allow users to search all campaigns for a certain keyword</li>
<li>Redesign tip submission form:</li> <ul>
<li>Use standard Bootstrap form</li> 
<li>Rewrite form in Python instead of PHP</li>
<li>Add location field - minimum viable product will use a zip code, will be integrated with Google Maps API in the future</li> 
</ul>
</ul>
Our project is going in directions I would have never even imagined a semester ago, and I am very excited for the upcoming release!