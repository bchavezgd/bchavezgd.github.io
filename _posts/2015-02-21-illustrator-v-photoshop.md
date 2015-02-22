---
layout: post
title: "Why I think Illustrator is better than Photoshop for mocking up websites."
date: 2015-02-21
category: opinion
tags: photoshop, rants, opinions
image:

---

Designers all have their own choices when it comes to tools of choice, the only thing really constant is the fact Photoshop has been used for almost anything that involved graphics or images. its like the Swiss Army Knife. We should rethink that, maybe we (as designers) should think of things like Photoshop as a single tool, instead of a tool box. From what I can tell, Photoshop is still the first tool many designers go to for mocking up a website. I think that this can be improved on. I believe that Illustrator is better for several reasons. I know this will be a very subjective article, but I hope that people will read the article and try it out before dismissing the idea.

*Please note through out most of this article I refer to CS6 unless otherwise specified.*

## Lets start with the Pros:

**Photoshop**

- More popular, therefore easier to collaborate.
- Photoshop can handle exporting in many different file formats.
- Can create animated GIFs natively.
- The color picker is one of the best I've come across with the ability to handle Hex code, RGB, HSL, LAB, and CMYK, inputs and outputs.
- it's pretty familiar for most designers.
- highly portable.
- backwards compatible files with older versions of the software.
- embedding images as layers, or smart object.

**Illustrator**

-  SVG is a native file format.
-  Like Photoshop, it can also export JPG, PNG, and GIF. and many other formats.
-  Art boards. *this is big.*
-  Linking files simulates the way websites link to images.
-  cleaner typography, editing and exporting.
-  smaller file sizes
-  less system resources used while designing.
-  can export smaller graphical items easily.
-  auto-grouping layer system
-  easy color theme switching.

## Now some Cons:

**Photoshop**

- Large file sizes.
- needs more system resources.
- can't export smaller graphical components easily.
- need to be more diligent about layers and grouping to stay organized.
- static canvas sizes.
- not as easy to work with multiple canvases on the same screen.
- no SVG support.

**Illustrator**

- Less popular, so being able to hand off files becomes harder.
- Less portable files when images are linked.
- Creating animated GIFs isn’t native, requires third party dependencies.
- Files aren't as backwards compatible like .PSD files
- Can't edit raster images.


---

Now that the list is out of the way lets unpack some of these.


### Collaboration and Portability

Photoshop is already the industry's go to for mocking up a website, meaning that you can be pretty sure that when you're handing off a file, it's going to someone that expects a PSD file. However, Illustrator isn't widely used as a mockup tool so not many people will expect it to be used as such. Also the advantage with Photoshop is the fact that all the images would end up being embedded to the file as either a smart object, shape layer, or rasterized layer. So handing it off is easy, you just save out the PSD, and done, it's only one file to worry about. where as an Illustrator file needs to include whatever linked images it may rely on, but I find this interesting. When I started doing web design the first thing I learned was the file system is pretty sensitive. that sensitivity is replicated with an Illustrator file that has linked files. I like this, here's why. I will only use Photoshop to edit photos and any other raster images, trying to use Illustrator to do the same edits is not worth the time or effort. I don't want to edit vector items in Photoshop when Illustrator is more efficient. It's not uncommon for me to have both Illustrator and Photoshop open at the same time. Going back and forth isn't that hard. Why would I want to waste system resources just to have a layered PSD file open when I only need the final product to be displayed in my AI file? Since I can't really think of a good reason I choose not to keep however many heavy files open unless I'm actually working on it. Finally here's why Illustrator wins this one in my opinion.

**Folder setup**

When sending a Photoshop file it may look like this (pre CC).

![]({{ site.url }}{{ site.image-folder }}/file-sys-00.jpg)

Whereas the an Illustrator file would look like this (ignore the notes folder because i don't know many people that do that).

![]({{ site.url }}{{ site.image-folder }}/file-sys-01.jpg)

so lets compare each to a how the working HTML/CSS mockup would look like (simplified of course).


    /mockup folder
        > index.html
        > style.css
        > fonts folder
            > files
        > IMAGES
            > image1.jpg
            > etc.jpg

Notice that the images folder needs to be there with the HTML documents. When sending a file with linked images it'll be there by default. This alone should be something to consider when thinking about work flow from mockup to functional prototype. *In CS6 they actually start to act the same, where when you go to `File > Place..`. an image into either program, they link by default. Previously in Photoshop it would embed as a layer.*

---

### SVG and File Exporting

Another reason that I prefer Illustrator is the fact that SVG are quickly becoming a usable and reliable format for web graphics,  from icons and buttons to animations with canvas or JavaScript, SVG aren't going away anytime soon. since they are a vector format Photoshop *shouldn't*. Illustrator, however, works perfectly with them. it does have shortcomings but optimizing an SVG isn't exactly hard. Since they are scalable up or down, they won't degrade when being stretched if needed. which would be something that would happen with raster files like PNG's that would be used for the same icons and whatnot.

---

### Typography

It's no secret that Illustrator handles type way better than Photoshop does, especially longer blocks of text. Photoshop should only use text editing for headlines or complicated type treatments. Smaller blocks are easier to edit in Illustrator, and change their settings, including the size of the containing box. In practice this is a very small issue so I think the only advantage is when embedding text into an SVG graphic, you'd get a cleaner final product than rasterizing it in a PNG. but the main reason I think Illustrator wins this one is because to change a color or font setting is simple as clicking on the word or text block and while the menu is open, which is usually one click less than Photoshop. two clicks less than trying to change a color in Illustrator vs Photoshop. Its more intuitive to click a text block to select it, than to hunt and select the layer to make the same changes.

![Illustrator]({{ site.url }}{{ site.image-folder }}/ill-typo-00.png)

Also, its much quicker to try different type combinations to figure out what will suit your project.

![]({{ site.url }}{{ site.image-folder }}/ill-typo-01.jpg)

---

### System Resources.

Photoshop is a heavy program on your computer, it'll slow your computer down to a crawl depending on how large your file gets. This is due to the fact that you're relying on raster graphics which eat up your computers memory, and in-turn slow it down. This to me is incredibly annoying. Since Illustrator relies on vector graphics and simple previews, it doesn't need as much memory to display what you need, leaving the free memory to speed up your computer overall.

Secondly a PSD file can easily reach 50+MB, whereas a AI hardly ever gets above 1mb. So yea Illustrator wins again.

---
### Artboards

Illustrator has the advantage of artboards that can export there own individual graphics, from the same file. Lets say you design a handful of icons in the same file, if you where using Photoshop you'd end up having to separate them into their own files before exporting them as usable files, or a sprite grid, a new feature in Photoshop CC is the "Extract Assets" which is similar to art board exporting but since I'm still running CS6 at home and haven't used it at work I can't speak for its performance. Illustrator, you can just wrap each icon or graphic within a new artboard and then export it all from one file by selecting a single check box.

![]({{ site.url }}{{ site.image-folder }}/ill-artboards-icons-00.jpg)

For a demo, 3 quick icons that could be used as UI elements. Each in their own artboard. This makes it easy to save out as multiple files when "Use Artboards" is checked.

![]({{ site.url }}{{ site.image-folder }}/ill-artboards-icons-01.jpg)

I love this for its efficency alone. 

#### Designing Above The Fold

Another advantage of the artboard is the fact that you can design *around* it. During the initial development of my designs I'll have a lot of build items around the artboards as a way to work on stuff that wouldn't need to be in the final product, but needs to be built separately. Another use would be when designing below your artboards so you can see how a page would scroll, and what needs to happen below the fold of your site.

![artboard]({{ site.url }}{{ site.image-folder }}/artboards.png)

In Illustrator, you can keep designing down beyond the fold at will. Whereas in Photoshop, you have to extend the canvas which is a two step process, with or without knowing the hot-key for it.

![]({{ site.url }}{{ site.image-folder }}/ps-canvas-00.jpg) ![]({{ site.url }}{{ site.image-folder }}/ps-canvas-01.jpg)


#### Designing for Media Queries

Responsive design is unavoidable now. seeing as most people use a device that’s not a computer to browse the web, tablets and smart phones have to be considered when designing your website. So to simulate the screens you can start a Photoshop file with a PPI matching the devices and dimensions, for each media query you'd have to design for, at minimum two but can be upwards of four. With Photoshop that would end up being one file per media query. In Illustrator you can have your multiple media queries all in one file, via artboards this is convenience since you have all the media queries right in front of you on the same screen.

A similar consideration would be off canvas navigation for smaller screen media queries, or even just how your layout can change when going from desktop design to smartphone.

Another win for Illustrator for simplicities sake.

---

> “You must be shapeless, formless, like water. When you pour water in a cup, it becomes the cup. When you pour water in a bottle, it becomes the bottle. When you pour water in a teapot, it becomes the teapot. Water can drip and it can crash. Become like water my friend.”
> 
> ― Bruce Lee

### Honorable Mentions

There are new competitors with [Sketch 3](HTTP://bohemiancoding.com/sketch/), I haven't used it because it's OSX only (I don't have a mac, because they are insanely over priced) the software itself is only $99 for the license, so that's good. Adobe has more than one capable tool with their new Creative Cloud service [Adobe Muse](HTTP://muse.adobe.com/) and [Edge Reflow](https://creative.adobe.com/products/reflow), both are worth looking in to, but their cost of admission at $600 a year for the CC subscription is pretty high. Their is also [Serif's Affinity Designer](https://affinity.serif.com/en-gb/), which again is mac only but only about $50 (£39.99 offically).

### Final Results

Well its pretty clear that I think Illustrator is a better tool for mocking up a website and I hope that I change a mind or two. That's not to say that Photoshop is without it's own merits. I just believe it's a photo editing tool, not a web design tool. A few places Photoshop is better is file compatibility, you can make a PSD in CS6, and it'll open in CS4. You can't reliably do that with Illustrator. And since it's the go to software already, there are tools that use a PSD to convert them to HTML/CSS files without knowing much code. And finally, it's your decision not mine, but try it. You might like it.