---
layout: post
title: "Getting Checked In"
featured-img: check-in
type: home
mathjax: true
---
# Our check-in process

By now you should have recieve a couple emails in regards to your booking. Do take note of the important details mentioned in that brief listed on the right. The information will help ensure you trip to the house from the airport or another part of the island is a smooth and well informed trip. We don’t want you rocking up flustered already.

**Important info to note down**
* Your room name
* The number for security +62 821 4745 3614
* The house managers’ number +1 901 634 8275
* The house rules listed below
* Joining our Facebook group and Slack channel

## Once you arrive at Outsite

Either Robert, the house manager, or a member of the staff outsite staff will show you your room and offer you a cold wash cloth, coconut and SIM card if requested.

Who ever greets you should show you how the lock box works and explain the room cleaning schedule. In case they don’t, just call Rob WA +1 901 634 8275.

## After you unpack your bags

Go ahead and connect to the WiFi, pop in the SIM card so you can hotspot or do any number of other things that require data.

In our lobby you will find a massive chalk board. If you name isn’t already ready there, then add it to the list and let us know where you are from.

You can also look over the other information scribble on there in case the chalkboard has been update faster than this wiki.

If you need to get around town immediately, then hopefully you let us know to begin sourcing a scooter for you. Advanced notice definitely speeds up the process. Otherwise, let us know and hang out by the pool with your cocnut while we get you a pair of wheels.

Not used to riding a motorbike? We can arrange for you to get scooter lessons to give you more confidence when riding around town. It isn’t as bad as it might seem, I promise.

**Apps we recommend downloading**
* WhatsApp
* Go Jek
* Work Hard Anywhere
* Workfrom
* Slack

## In preparation for the day ahead
If you want breakfast you will want to submit your breakfast order form before 7pm. If you arrive after 7pm and a staff member is around you can try slip your order into the system through that back door. Otherwise, get Robert to show you the good local cafes. There are so many!

With all that out of your way it’s time to plan out your adventures.

### Posts

Create a new Markdown file such as `2017-01-13-my-post.md` in `_post` folder. Configure YAML Front Matter (stuff between `---`):

```yaml

---
layout: post #need to be post
title: Getting Started with Sleek #title of your post
featured-img: sleek #optional - if you want you can include name of hero image
---

```

#### Images

In case you want to add a hero image to the post, apart from changing `featured-img` in YAML, you also need to add the image file to the project. To do so, just upload an image in `.jpg` format to `_img` folder. The name must before the `.jpg` file extension has to match with `featured-img` in YAML. Next, run `gulp img` from command line to generate optimized version of the image and all the thumbnails. You have to restart  the jekyll server to see the changes. Sleek uses (Lazy Sizes)[https://github.com/aFarkas/lazysizes] Lazy Loader for loading images. Check the link for more info. Lazy Sizes doesnt't require any configuration and it's going to be included in your bundled js file.

### Pages

The home page is located under `index.md` file. To change the content or design you have to edit the `default.html` file in `_layouts` folder.

In order to add a new page, create a new html or markdown file under root directory or inside `_pages` folder and link it in `_includes/header.html`.

### Images TODO

Introduce gulp optimization

Breakpoint | Image Type | Width | Retina
------------ | ------------ | ------------- | -------------
xs |Post Thumb | 535px | 1070px
sm |Post Thumb | 500px| 1000px
md |Post Thumb | 329.375px | 658.75px
lg |Post Thumb | 445.625px | 891.25px
xl |Post Thumb | 353.125px | 706.25px


Breakpoint | Image Type | Width | Retina
------------ | ------------ | ------------- | -------------
xs |Post Hero | 535px | 1070px
sm |Post Hero | 500px| 1000px
md |Post Hero | 329.375px | 658.75px
lg |Post Hero | 445.625px | 891.25px
xl |Post Hero | 353.125px | 706.25px

### MathJax

If you want to use [MathJax](https://www.mathjax.org/) in your posts, add `mathjax: true` in [YAML front matter](https://jekyllrb.com/docs/frontmatter/) of your post:

```yaml
---
layout: post
title: Blog Post with MathJax
featured-img: sleek #optional - if you want you can include name of hero image
mathjax: true #add this line in order to enable MathJax in the post
---
```

#### Example:

In N-dimensional simplex noise, the squared kernel summation radius $r^2$ is $\frac 1 2$
for all values of N. This is because the edge length of the N-simplex $s = \sqrt {\frac {N} {N + 1}}$
divides out of the N-simplex height $h = s \sqrt {\frac {N + 1} {2N}}$.
The kerel summation radius $r$ is equal to the N-simplex height $h$.

$$ r = h = \sqrt{\frac {1} {2}} = \sqrt{\frac {N} {N+1}} \sqrt{\frac {N+1} {2N}} $$
Happy hacking!
