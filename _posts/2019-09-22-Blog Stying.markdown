---
layout: post
title:  "Styling Blog With a Custom Template"
date:   2019-09-22
---

<!-- <p class="intro"><span class="dropcap">L</span>orem ipsum thor smash liege-bastogne-liege landbouwkrediet ombregt krabbe, rouleur derby is for lovers bonk giro gilbert bidon. Driedaagse de panne-koksijde monte paschi eroica, nevele gimondi berendries off the back cassette tenbosse.</p> -->

When I started to style this blog using a custom template, I downloaded a template from [this website](https://www.wowthemes.net/jekyll-themes-templates/). I looked at various templates available and chose to downloaded a template called "Long Haul", which you can find on GitHub via this [link](https://github.com/LevytsRoman/levytsroman.github.io).

I liked this template mainly because of how well styled it is.
Bellow are two screenshots I took after running the project locally on my computer.

1. **Screenshot for Navigation Bar and Header Sections**
<img src="{{ '/assets/img/header and title.JPG' | prepend: site.baseurl }}" alt="">

2. **Screenshot for Content and Footer Sections**
<img src="{{ '/assets/img/footer and content.JPG' | prepend: site.baseurl }}" alt="">

Even though, It worked eventually, I had trouble integrating this template in my original blog because I tried to manually edit different files
trying to add css and javascript files provide by the template. After trying and failing, I realized that copying and pasting the _includes, _layouts assets, and css folder of the template into the root directory of my blog would get the job done.

I am still not sure how to add a plain css boostrap template, but I guess I will learn this in the next step, and that is what I look forward to.
