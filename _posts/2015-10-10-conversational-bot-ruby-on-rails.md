---
layout: post
title:  "Make a conversational bot in Ruby on Rails from scratch."
date:   2015-10-10 15:30:00
categories: bot ruby rails
image:
  feature: header-image.png
---

Hi everyone! For the first post on my Github's page I was wondering what could I do
to make something fun and useful, so I end with this idea: **make a conversational
bot in Ruby on Rails**.

Since I start to study about artificial intelligence some
years ago, one of the most interesting fields of this computer science's area
for me was the [automated online assistants](https://en.wikipedia.org/wiki/Automated_online_assistant).

The first approach I found that was kind of simple was [AIML](https://en.wikipedia.org/wiki/AIML),
or **Artificial Intelligence Markup Language**. Is a XML dialect that helps you
to create natural language bots, developed between 1995 and 2002.

## Let's see an extremely short introduction to AIML

Because all the details about the **AIML** syntax and usage is properly documented
on the [Alicebot](http://www.alicebot.org/aiml.html) website, we're going to see the
basis in order to be able to do our very simple first bot.

On this piece of code we have the *Hello wold!* of **AIML** (kind of):

```xml
<aiml version="1.0.1" encoding="UTF-8"?>
   <category>
      <pattern> HELLO MY BELOVED BOT! </pattern>
      <template>
         Hello my friend! :)
      </template>
   </category>
</aiml>
```

As you could see, matches with any **XML** dialect, having tags, elements and
attributes (well, on this example we don't have attributes).

So, let's see on detail the elements we have on this example:

### Tags

* `<aiml>`: defines the beginning and end of a **AIML** document.
* `<category>`: defines the **unit of knowledge** in bot's knowledge base.
* `<pattern>`: defines the pattern to match what a user may input to a bot.
* `<template>`: defines the response to user's input.

## But... why this should be fun?

Well, apart from the fun that implies learn new things, we could do a conversational
bot of anything, so let's do one with your favorite humorist. In my case, this is
the Spanish humorist [Chiquito de la Calzada](https://en.wikipedia.org/wiki/Chiquito_de_la_Calzada):

![Chiquito de la Calza](/images/2015-10-10-conversational-bot-ruby-on-rails/chiquito.gif)

*Chiquito de la Calzada in all his glory. Please don't fall hipnotyzed by the gif,
I know is hard, but let's continue.*
