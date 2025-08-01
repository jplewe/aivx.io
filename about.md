---
layout: page
title: about
permalink: /about/
---

### contact/socials

email: hi at aivx.io  
x/twitter: [aivx_io](https://www.x.com/aivx_io)  
linkedin: [john plewe](https://www.linkedin.com/in/johnplewe/)   
instagram: [aivx_io](https://www.instagram.com/aivx_io)  


### about me

I’m John Plewe, a creative software developer and occasional game designer. Most of my work has been at [Nevercenter](https://nevercenter.com) as part of a three-person startup (two devs). A good place to get an overview of my various projects, awards, achievements, etc. is via [LinkedIn](https://www.linkedin.com/in/johnplewe/) (feel free to add me there, my friend count is dismal), though it doesn't include some fun life highlights like getting surprise-offered a job by Valve's Gabe Newell in his office full of knives, or brought out by Apple to develop CameraBag on heavily-secured iPads at their HQ pre-launch.


### about AIVX

**AIVX** is my new solo company and label for my creative work. For now, it's focused around the new generative 3D engine I'm developing, which I'll use to build games, creative tools, virtual worlds, live DJ visualization apps, a holodeck, and much more. I'm very excited to get going with it. I have accounts on [X](x.com/aivx_io) and Instagram.

If you're curious about the name itself, it comes from a project naming convention I found myself using (_ax for audio experiments, _ix for interactive, _vx for visual). I wanted to follow the xkcd theory of naming. I also wanted something short and unique enough that I could stick it in front of all my app names and not have to think too hard about coming up with names. Mission accomplished.

### posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> – {{ post.date | date: "%B %-d, %Y" }}
    </li>
  {% endfor %}
</ul>