---
draft: false
author: "Marga"
title: "Metrics"
date: "2024-11-18"
description: ""
---

![TelemetryDeck countries graph, showing 16.67% users coming from each of the countries United States, Netherlands, Moldova and Germany. The remaining 33.3% is from Cambodia.](/post/2024/11/metrics/telemetrydeck-countries.jpeg "TelemetryDeck countries graph")

It's always fun to see if people visit your site or blog. It can be useful too, so you know what subjects are popular. I mostly just write for fun, but if you're aiming for results, you're going to need some data.

#### TelemetryDeck

The minute you're adding analytics tools to your site or app, however, you're dealing with your visitor's / user's privacy. I prefer to use tools that treat user data with care. In the case of this blog, which is made with [Hugo](https://gohugo.io), I'm now using [TelemetryDeck](https://telemetrydeck.com). I like that TelemetryDeck does not collect [any personally identifiable information](https://telemetrydeck.com/privacy). On top of that, up to 100K signals per month, it's free to use. (And no, I don't have stocks, I just really care about privacy, and I know the people at TelemetryDeck do too!)

#### Implementing TelemetryDeck on Hugo

I started by reading their [Web Setup Guide](https://telemetrydeck.com/docs/guides/web-setup/) which looked really simple and easy. I cheered a bit too soon, because I couldn't find how to add a script to the `<head>` section of every page.

What I ended up doing - and I *think* this works for all Hugo themes - is this:

- In the root of your repo, find the folder named `themes\<your-theme>\layouts\partials\` (in my case `<your-theme>` is `hugo-flex`)
- Copy the file `load_site_assets.html` from there to `layouts\partials\load_site_assets.html`
- Open the file, go to the bottom, add a newline, and add put the script that's mentioned in the Web Setup there.
- Save, commit, push, and done!

As ever so often, figuring this out was more work than actually pasting it in.

