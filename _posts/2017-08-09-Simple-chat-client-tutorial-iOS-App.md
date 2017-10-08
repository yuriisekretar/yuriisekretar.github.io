---
layout: post
title: "Chat Client Tutorial: Simple iOS Application"
---

> "A single mediocre hire within the first five will often in fact kill a startup." - Sam Altman.

That's why you should treat hiring with same level of importance as developing your product.

One of the steps I usually have is a skills assessment test. This tutorial will show how an ideal candidate should approach and complete task been assessed for Junior iOS Software Developer position. One of the tasks I usually choose is Simple Chat Client. Final project will show skills as understanding UI Guidelines, implementing complex apps, working with 3rd party libraries, handling multithreading and general language skills.

### Assesment task example
- _User Interface:_ two main screens Login and Chat
- _Error handling:_ wrong username/password, no Internet connection, empty values
- _Multithreading_: send/receive messages without blocking UI
- _Infrastructure:_ XMPP or WebSocket public servers
- _3rd Party Library_: should be used to implement communication protocol

## User interface

"Should software developers understand principles of UI/UX design?" I have heard this question asked over and over again working side by side with designers and developers.

Apple created Human Interface Guidelines for this reason. As an app developer, you have the opportunity to deliver an extraordinary product that rises to the top of the App Store charts. To do so, you'll need to meet high expectations for quality and functionality.

Candidate for a position will be provided with a design implemented in Sketch. And while in the future candidate will work side by side with designers he should understand how to use and read Sketch designs.

Simple Chat Client will have only two screens.

![chat-client-design](/public/posts/chat-client-design.png)

[Download Sketch file](/assets/task.sketch)

Login screen should have two text fields, handle empty or wrong data entry and Internet connection problems.

Chat screen should have incoming/outgoing messages list, multiline message text field, text field with recipient username and logout button.

## Getting Started

To get started create Single View App XCode project and open Main.storyboard in the Interface Builder. Remove default View Controller Scene and replace it with Table View Controller and set it as Initial View Controller. We will use it to implement Login screen. Table View makes it easier to handle text entering, different screen sizes and interface looks simple and clean.

Set Table View Content type to Static Content and Style to Grouped. By default there are three cells present under Table View Section, delete one as we will need only two for Username and Password.

![chat-client-design](/public/posts/chat-client-getting-started-login-screen-1.gif)

### Authentication





### Implemenation

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.


Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis lorem ut libero malesuada feugiat. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur aliquet quam id dui posuere blandit. Nulla quis lorem ut libero malesuada feugiat. Nulla porttitor accumsan tincidunt. Pellentesque in ipsum id orci porta dapibus. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.

Quisque velit nisi, pretium ut lacinia in, elementum id enim. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Pellentesque in ipsum id orci porta dapibus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula. Vivamus suscipit tortor eget felis porttitor volutpat. Pellentesque in ipsum id orci porta dapibus. Nulla porttitor accumsan tincidunt.

Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Sed porttitor lectus nibh. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula. Nulla quis lorem ut libero malesuada feugiat. Sed porttitor lectus nibh. Curabitur aliquet quam id dui posuere blandit. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum congue leo eget malesuada. Curabitur aliquet quam id dui posuere blandit.

Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula. Donec sollicitudin molestie malesuada. Vivamus suscipit tortor eget felis porttitor volutpat. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui. Donec rutrum congue leo eget malesuada. Nulla porttitor accumsan tincidunt. Vivamus suscipit tortor eget felis porttitor volutpat. Vivamus suscipit tortor eget felis porttitor volutpat. Quisque velit nisi, pretium ut lacinia in, elementum id enim.

Nulla quis lorem ut libero malesuada feugiat. Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Donec sollicitudin molestie malesuada. Nulla porttitor accumsan tincidunt. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis lorem ut libero malesuada feugiat. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Nulla quis lorem ut libero malesuada feugiat.
