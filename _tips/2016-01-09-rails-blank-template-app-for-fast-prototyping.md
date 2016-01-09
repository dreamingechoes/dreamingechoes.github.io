---
layout: tip
title: "Rails blank template App for fast prototyping."
date: 2016-01-09 15:30:00
categories: bootstrap ruby rails
tags: gem ruby rails development web bootstrap theme admin prototyping
comments: true
excerpt: "If you need to do some quick prototype on Rails of an idea or whatever, here is a simple Rails blank template app in order to be able to just simply clone it and start to develop your own app..."
tip_summary: "If you need to do some quick prototype on Rails of an idea or whatever, here is a simple Rails blank template app in order to be able to just simply clone it and start to develop your own app..."
image:
  feature: header-image.png
url: /tips/2016-01-09-rails-blank-template-app-for-fast-prototyping/
---

If you need to do some quick prototype on Rails of an idea or whatever, here is a simple Rails blank template app in order to be able to just simply clone it and start to develop your own app.

It uses the Bootstrap SB Admin Base V2 theme. You could find the Rails gem of this theme [here](https://github.com/dreamingechoes/bootstrap_sb_admin_base_v2).

Main features included by default:

- [Devise](https://github.com/plataformatec/devise) with default modules.
- [BootstrapSBAdminBaseV2](https://github.com/dreamingechoes/bootstrap_sb_admin_base_v2) theme included.
- [SendGrid](https://github.com/stephenb/sendgrid) gem for mailing.
- Continuous testing with [Guard](https://github.com/guard/guard).
- Thin server.
- MySQL database.
- ERB template engine.

There is an user example ready to use to login with email `user@example.com` and password `123456789`.

![screenshot](/images/2016-01-09-rails-blank-template-app-for-fast-prototyping/screenshot1.png)
Login page.

![screenshot](/images/2016-01-09-rails-blank-template-app-for-fast-prototyping/screenshot2.png)
Dashboard page.

Here you have the [Github repo](https://github.com/dreamingechoes/rails-blank-template-app) for this template, so you can clone it, change it, play with it... whatever you want! :)
