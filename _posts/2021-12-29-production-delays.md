---
title:  "Production delays"
categories: 
---
I've basically completed my Twitter clone -- it's fully functional in **development** mode. 😃 Besides tweeting, liking, and retweeting, it fetches recent webdev tweets from the Twitter API and displays them in the feed: 

<img src="/assets/images/tweeter-border1.png" alt="screenshot" style="height: 400px;">    <img src="/assets/images/tweeter-border2.png" alt="screenshot" style="height: 400px;">

It's ready for production, ie. being hosted so that you can use it. But I've hit a snag... apparently the Twitter API doesn't support CORS headers, which are related to internet security. What this means for me is that I can't fetch tweets directly from my front end app. The requests need to come from a server, which *was* outside the scope of the project. 🤔 Now I'll have to fix that.

Bottom line, I celebrated a bit too early and now I'll need to spend some more time learning about how to get it fully up and running. I'll be over here looking into the fascinating world of middleware and serverless functions. Stay tuned!