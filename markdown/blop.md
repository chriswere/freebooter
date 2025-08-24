---
date: 2025-08-17
title: A blop in the bucket
---

Much like [Liz Truss](https://www.huffingtonpost.co.uk/entry/liz-truss-tank-estonia-margaret-thatcher_uk_61a60ddfe4b025be1aee877e) driving a tank into Estonia, I'm going to do something confusing and likely foolhardy: rebuild the pride and joy of my digital presence with [Drew's](https://friendo.monster) static website builder, [blop](https://gitlab.com/uoou/blop). I'm a big lover of static sites for all the use cases you can apply them to. They're faster, more stable, more portable, require fewer dependencies and resources, and you generally have more control over them when it comes to administrative tasks. Fellow [Space Virgin](https://video.thepolarbear.co.uk/c/expanse/videos), [Hamish the Polarbear's website](https://thepolarbear.co.uk), is also static, being a gentleman of refined taste and all.

So, what is this blorp?

Firstly, it's 'blop'. Secondly, the project page defines blop succinctly: "blop essentially just converts markdown into HTML in a lightly structured way. Run blop in a directory where you want the local copy of your blog to live and then upload/push the resulting HTML to your website." Thirdly, the Urban Dictionary defines blop thusly: "[the sound of jelly when it falls off your knife onto the floor](https://www.urbandictionary.com/define.php?term=blop)." Please don't look at the subsequent definitions, you won't like them.

I wanted to get back into writing, make my website somewhere more interesting to visit, and align myself with the small/smol web. Every now and then, I want to tinker with this little facet of my personality. The last time I made a significant change here was the new 'picnic style' theme. I considered giving Hugo and E11y a shot, but they both felt like more than I needed. Additionally, Drew had been keeping blop ticking over for years now, and it always seemed to work well for him. I mean, all I need is something to convert .md files into an HTML template and assemble an RSS feed.

The RSS feed was important, in fact, I was even considering creating an RSS feed-only blog at one point. I've recently been getting into [Newsboat](https://newsboat.org), a command line RSS reader that fits the way I like to read perfectly. People have been recommending [Newsraft](https://codeberg.org/newsraft/newsraft), but I've yet to give that a go. I tend to opt for what's available in the Debian stable repositories as a broad, albeit sometimes broken, rule.

Not many people get the privilege of having the creator of a piece of software available to personally offer a step-by-step guide on getting all the templates set up, but Drew, being one of the kindest people I know and one of my best friends, took the time to get me set up nicely, even though he was having a migraine (or, as I like to call them, blood attacks).

I managed to migrate a lot of my old website content over very easily, as is the beauty of working with plain text. I never cared much for having too many images on my website, waste of space and bandwidth if you ask me.

All in all, blop is everything I need and want out of a static site generator, and I'm incredibly grateful to Drew for putting it together. I've even made myself a little script to push the changes easily. Due to this new workflow, I'm now hosting this site on [Codeberg Pages](https://docs.codeberg.org/codeberg-pages).

So, how does it work?

Well, you simply pull all the files from the [blop project page](https://gitlab.com/uoou/blop) using git, or a web browser if you prefer. Adjust the templates, style.css, url.txt, site.conf, and add your posts in the form of markdown files in the markdown folder, then run blop. Sidenote: I've placed blop in my ~/.local/bin folder, where I keep all my local executables, but you can stick it anywhere you like. The [full documentation](https://gitlab.com/uoou/blop/-/blob/master/README.md) has all the settings options as well as details on how to get your blop site set up properly.

To top it all off, I've set up a little script that compiles the site and pushes it up to Codeberg. While the script is very basic, all of my work can be seen on the [Codeberg project page for my site](https://codeberg.org/ChrisWere/pages). A big thanks to Codeberg, by the way, for being such a wonderfully supportive institution in the free software and open-source world, as well as a big thank you to Drew for taking the time to put together this tool and walk me through using it.
