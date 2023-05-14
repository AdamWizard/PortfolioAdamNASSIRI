---
title: "Extra Leaderboards API"
date: 2023-05-01T18:29:28-04:00
draft: false
tags: ["projects","Java"]
---


{{< lead >}}
{{< typeit 
speed=50
lifeLike=true
>}}An API that provides data for a trackmania plugin, it's all about going faster.
{{< /typeit >}}
{{< /lead >}}  

## Speeding up the plugin

The [Extra Leaderboard positions plugin](https://github.com/Banalian/ExtraLeaderboardPositions) is an existing plugin for trackmania that allows players to get more information about their placement on a given map.

The goal of **integrating API usage** to the existing plugin was to make it **more responsive** by getting a response from the ubisoft API faster.

The result is [this project](https://github.com/Banalian/ExtraLeaderboardAPI), that uses an amazon webservices machine to handle the requests from players and forward them to the ubisoft API, then send ubisofts response back to the user.

## My part of the work
### The Chain of responsibility
I was in charge of the backend part of the program running on the AWS machine, developping methods to translate the API responses, convey them from users to the ubisoft API, and then back to an instance of the plugin on the users side.

The main part of my job was making the responsibility chain that is used to process the replies we get from Ubisoft.

## Conclusion
This project was a great opportunity for me to learn more about `Java`, `AWS`, and the overall inner workings of an **API**.