---
layout: post
title:      "CLI Scraper Project"
date:       2021-04-27 13:48:09 +0000
permalink:  cli_scraper_project
---


Time for the first big project! I was incredibly excited to put what I've learned to work in designing my own app. I brainstormed over on good but simple CLI/scraping applications when the best idea struck me - what about an app that lets you search the UNESCO World Heritage sites for your next trip! A way to marry my love of culture and coding at the same time! Perfect, right? 

Well, the internet Gods spoke and it turns out some sites make scraping an absolute nightmare. After parsing through the HTML on the original UNESCO site and having issues pulling elements because of the way they were grhttps://www.visittheusa.com/experience/world-heritage-sites-united-statesouped/classed, I decided to find another website that was slightly more scrapable. I came across [World Heritage Sites in the United States](https://www.visittheusa.com/experience/world-heritage-sites-united-states), whose HTML was written in a very clear and concise manner. I decide to make my original idea a little simpler using this site to create a CLI that allows the user to see a list of all 24 UNESCO World Heritage Sites in the US and then select which site they want to learn more information about. 

This idea seemed to work a lot better and I had the basic CLI/scraper/site working shortly thereafter. The next difficult step was making sure I had the gem build correct. For whatever reason unbeknownst to me, I did not catch the "bundle" gem that basically sets up your gem files for you, so I was trying to create them from scratch. After much headache, I found this [gem](https://www.youtube.com/watch?v=XBgZLm-sdl8&ab_channel=Learn.co) (pun intended) and at 1:14:00, Avi walks you through how to use 'bundle' to set up your gem files for you. This was super helpful and I had my new gem up and running shortly after. 

The last big hurdle was getting it to [my GitHub](https://github.com/chelsealandsky/CLI-Scraper-Project), which I did not foresee being an issue. Long story short, the files would push, but they would have an "Escape" after them and GitHub was yelling at me saying my checks had failed, including this very interesting rake:
![cliprojunesco_fail](https://twitter.com/Chelsealandsky/status/1386778003062013959/photo/1).

I'm still trying to troubleshoot the GitHub issue, but the program itself runs beautifully! Very proud of myself, as this was the first program/gem I created from scratch. The pain was definitely worth it in the end. I'm excited for more!
