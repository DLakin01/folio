---
layout: post
title: API Consumption
date: November 10, 2017
---

In the latest step of my Bloc course, I wrote a simple API client in the form of a Ruby Gem, called Kele Client. Although this was a very quick and relatively easy portion of the course, the skills I used and the things I accomplished with them really got me thinking. One of the ways I’ve been pushing myself throughout my program is to think beyond the visible portions of websites, since so much of what a developer is concerned with happens behind the scenes, as information gets pulled, acted on, and rendered for viewing.

Up until this point, the information I was working with was always local - a `Fixtures.js` file, a Ruby hash, or a local database populated entirely on my end. This marked the first time I used an API to consume data from an exterior source, and pull it, in a readable and accessible format, into my local environment. The format of Kele Client was very intuitive - it’s just a Ruby class, with an initialize method that sends credentials to your chosen endpoint, and other methods to pull specific resources.

The gem itself uses HTTParty and JSON parsing to communicate with Bloc’s own API, pulling down chunks of information in the form of a parsed JSON string. In the course of messing around with the API, there was one point where I thought I had gotten stuck - in an effort to clear up `kele.rb`, the main file of the client, I had moved several methods to a subfolder, and used `require` and `include` to let them be called from `kele.rb`. However, my Ruby console kept throwing errors, saying it couldn’t find the file! I checked again and again making sure the file path was declared correctly and that the code looked good.

Despite my efforts, I was still having issues. Then I thought to try a different console, Pry. Wouldn’t you know, it worked just fine! I also discovered that Pry prints out the returned JSON strings in a much more readable format. When it comes to consuming data in the future, I may continue to use Pry in the configuration stage, to make sure I’m getting what I want to get.

**APIdeas**
-	Set up an API client with an Alexa voter education/GOTV skill, so Alexa can stay up to date on new developments and election day information
-	Use an API client to pipe in data from a remotely hosted database for a data visualization/analysis project
-	Use APIs from social justice orgs to populate a “Where’s the protest” app?
