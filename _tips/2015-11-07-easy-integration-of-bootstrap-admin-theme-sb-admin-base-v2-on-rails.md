---
layout: tip
title: "Easy integration of Bootstrap Admin theme SB Admin Base V2 on Ruby on Rails."
date: 2015-11-07 12:30:00
categories: bootstrap gem ruby rails
tags: gem ruby rails development web bootstrap theme admin
comments: true
excerpt: "I need to integrate the Bootstrap based admin theme SB Admin 2 into a Rails application. I had search on the internet about a gem in order to make it easier the integration of all the assets (images, fonts, css, js…), and due to I didn’t found any gem, I developed a Rails gem of them.."
post_summary: "I need to integrate the Bootstrap based admin theme SB Admin 2 into a Rails application. I had search on the internet about a gem in order to make it easier the integration of all the assets (images, fonts, css, js…), and due to I didn’t found any gem, I developed a Rails gem of them.."
image:
  feature: header-image.png
url: http://dreamingechoes.github.io/2015-11-07-easy-integration-of-bootstrap-admin-theme-sb-admin-base-v2-on-rails/
---

I need to integrate the [Bootstrap based admin theme SB Admin 2](http://startbootstrap.com/template-overviews/sb-admin-2/) into a Rails application. I had search on the internet about a gem in order to make it easier the integration of all the assets (images, fonts, css and js), and due to I didn’t found any gem, I developed a Rails gem of them.

![Bootstrap based admin theme SB Admin 2 dashboard example](http://startbootstrap.com/assets/img/templates/sb-admin-2.jpg)

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'bootstrap_sb_admin_base_v2'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install bootstrap_sb_admin_base_v2

## Usage

After install the gem, the only thing you should do in your Rails application is add some lines into your manifests files. Add this into your `application.js` file:

```ruby
  //= require bootstrap_sb_admin_base_v2
```

and this line into you `application.css` file:

```ruby
  *= require bootstrap_sb_admin_base_v2
```

And you're ready to use the HTML structure of the Bootstrap based admin theme SB Admin 2 on your Rails application. All the details and documentation about this is [here](http://startbootstrap.com/template-overviews/sb-admin-2/).
