+++
draft = false
author = "Marga"
title = "Hacked"
date = "2024-11-03"
description = ""
+++

As I wanted to set up my new blog, I found that past me already created a repo on GitHub for it. There was only an index.html with the words "Hello world!". So far, so good. But when I used my custom domain name, I ended up on some vague gambling site, which was definitely not mine. Was I hacked? How was this possible, I set up 2FA everywhere?!

First I checked at my domain hosting provider (Hover). Everything looked normal there. And the direct link to my GitHub Pages looked fine too. I noticed that the custom domain name in the settings of my blog's repo wasn't filled in, so I did that, but couldn't save my changes. That domain name was already taken. WHAT?! This is *my* domain!

I now suspect that I never filled in the custom domain name that I had, because there was no real content on the blog yet. If someone (likely a bot or a script) then scans a list with domain names, checks if they redirect to a GitHub Pages IP address, and then notices there is no actual site connected, they can fill in that domain name on another GitHub Pages repo. There they can either host their site, or more likely, set up a redirect to whatever site they want to promote.

Luckily this can be avoided. For one, you should (apparently :sweat_smile:) always make sure that your custom domain name is filled in at your repo's settings, if you point your website to a GitHub Pages repo. Ideally, you should also [verify your custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages). That way only repositories owned by your personal account / your organization can be used to publish a GitHub Pages site to the custom domain or its immediate subdomains. Verifying my domain also meant that I could reclaim it. 