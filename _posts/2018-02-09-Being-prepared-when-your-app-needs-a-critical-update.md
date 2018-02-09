---
layout: post
title: "Being Prepared When Your App Needs a Critical Update"
description: "How to incorporate Firebase Remote Config into an application in order to notify users about a critical update."
---

In any application lifecycle, there can be a situation when all of the users will be required to download an update. There are a couple of reasons for that: a critical bug, the backend was changed, rebranding etc. I will use the following edge case: when the future use of an app is not possible without downloading a new version.

The first time a saw this notification was on the very popular (at that time) Uber app. When I opened the app to request a ride, I saw a full-screen notification about a required update. It took me just 2 minutes to update and I already was ready to continue using the new updated version.

Some important things to remember are being prepared and basing an implementation on a third party service. By embedding in the application an external cloud platform, you will mitigate the risk of changing your own API. But there is always the concern of how reliable the service you choose is. Google Firebase is a very powerful cloud platform with a good choice of useful products and it is reliable. One of the products is Firebase Remote Config. It allows you to modify an app without deploying it. This is ideal for our case as we need to dynamically incorporate a user interface that will lock application and explain to the user the necessity to download an update. The required code should be incorporated into the app from the first release.

## How it works
Firebase has ready-to-use libraries for a variety of platforms e.g. iOS, Android. It offers a simple interface where you work with Firebase parameters in the same way as local ones. But parameters can be changed using web-interface and pushed to the app immediately at any moment. To decrease the load on the servers Google suggests to use default fetch interval of 12 hours. Have this in mind when pushing new values.

## User experience
It is a good practice to display the update notification when a user is not in the middle of something. Identify moments when it is appropriate to display the message. Explain why an update is required and what benefits user will get after he will download the new version.

![github-email](/public/posts/update_app.png)

## Other use cases
As you understand, Remote Config is not only for pushing update messages to your users. There are other use cases where it can save you from releasing a new version of the application just for one tiny update. I would name only a couple of them:
- communicate to the users regular update messages
- update any images inside app e.g. a welcome banner for a special event or holiday
- setting up timers to test different approaches
- change a new features descriptions
- update Term of Service or Privacy Policy
- update urls to your backend

You can think about other use cases that will be appropriate for your app. But always have in mind - you should think ahead so your code will be in the app.
