+++
title = "Branch Web Presence"
+++
<!--: .wrap .size-70 ..aligncenter bgimage=images/pencil.jpg -->

## **Web Presence**

*How to get your business found on the web*.

---

## **What is Web Presence?**

In the context of your business, web presence refers to your businesses' presence on the internet.

- Your domain is the center.
-  
- 

---

## **What are your goals?**

The typical goals of a local service business are to *attract and book clients*.

We'll be working with these goals as we move through examples.

1. **The Hub**: Your domain + website. This serves as the foundation of a businesses' web presence.
2. **The Spokes**: External websites such as citation providers and social media. This helps direct potential clients to the hub, and also provides trust.

---

## **The Hub: Domain**

Once a business has a domain name, they have an almost infinite level of flexibility in what they can do with it. That's why it's so important to get right.

There are many providers ... suggestions:

- Namecheap
- Godaddy
- ?


---

## **The Hub: Hosting Provider**

The hosting provider chosen is somewhat dependent on what type of website you would like to create.

---



## **Hugo-Webslides**

Use markdown to write contents and render with [**WebSlides**](https://webslides.tv) to HTML.
{ .text-intro }

[{{< svg fa-github >}}Github](https://github.com/RCJacH/hugo-webslides)

---

<!--: .wrap -->

## **WebSlides Demos**
Here's what you can do with [WebSlides](https://webslides.tv).

- {{< gallery title="Why WebSlides" href="#slide=10" src="https://webslides.tv/static/images/demos-why.png" >}}Why WebSlides{{< /gallery >}}
- {{< gallery title="Landings" href="https://webslides.tv/demos/landings" src="https://webslides.tv/static/images/demos-landings.png" >}}Landings{{< /gallery >}}
- {{< gallery title="Portfolios" href="https://webslides.tv/demos/portfolios" src="https://webslides.tv/static/images/demos-portfolios.png" >}}Portfolios{{< /gallery >}}
- {{< gallery title="Keynote" href="https://webslides.tv/demos/apple" src="https://webslides.tv/static/images/demos-apple.png" >}}Keynote{{< /gallery >}}
{ .flexblock .gallery }

---
<!--: .wrap -->

## **More Examples**
<small>Note. None of these slides are currently ported to Hugo-Webslides...YET.</small>

- {{< gallery title="Netflix's Culture" href="https://webslides.tv/demos/netflix-culture" src="https://webslides.tv/static/images/demos-netflix.png" >}}Netflix{{< /gallery >}}
- {{< gallery title="Longform Articles" href="https://webslides.tv/demos/longforms" src="https://webslides.tv/static/images/demos-longforms.png" >}}Longforms{{< /gallery >}}
- {{< gallery title="Interviews" href="https://webslides.tv/demos/interviews" src="https://webslides.tv/static/images/demos-interviews.png" >}}Interviews{{< /gallery >}}
{ .flexblock .gallery }


---
<!-- : .wrap .size-40 -->

### **Configuration**

You can modify WebSlides settings directly from your project config.toml.
{ .text-intro }

~~~toml
[params.webslides]
  banner = false
  slideshow = true
  vertical = false
  autoslide = false
  changeOnClick = false
  disableLoop = false
  minWheelDelta = 40
  disableNavigateOnScroll = false
  scrollWait = 450
  slideOffset = 50
  hideIndex = false
~~~


---
<!-- : .wrap -->

|||v

### **All from one markdown file**

Use three dashes "<code>-</code>" to create a separate slide page.

|||

~~~md

Slide1

---

Slide2

~~~

---
<!-- : .wrap -->


|||

~~~
content
├── home
│   ├── home1.md (weight: 1)
│   └── home2.md (weight: 2)
└── _index.md (initial page)
~~~

|||

### Or not.

You can combine and arrange files with the weight parameter in front matter, and categorize .md files into different folders.

---
<!-- : .aligncenter -->

## Slide Attributes

Assign attributes to a slide by using the following notation.

~~~
---
<!-- : .class .class2 ..sub-class bg=bg-class bgimage=(frame|dark|light)|http://image-url/ bgpos=POSITION -->
~~~

~~~html
<section id="section-x" class="bg-class slide current" style="">
  <span class="background-POSITION" style="background-image:url('http://image-url/')"></span>
  <span class="background frame"></span>
  <div class="class class2">
    <div class="sub-class">
      CONTENT
    </div>
  </div>
</section>
~~~
---
<!-- : .wrap -->

### Assign class to elements

note: ***depreciated*** with the introduction of [Hugo's native block attribute](https://gohugo.io/news/0.81.0-relnotes#attribute-lists-after-markdown-blocks)

- {{< flexblock "Headers and Paragraphs" 6 >}}
<span># <!-</span>- : .hClass -<span>-></span>Header<br>
<span><!-</span>- : .pClass -<span>-></span>Paragraph
~~~html
<h1 class="hClass">Header</h1>
<p class="pClass">Paragraph</p>
~~~
{{< /flexblock >}}

- {{< flexblock "Lists" 6 >}}
<span><!-</span>- : .listClass -<span>-></span><br>
<span>-</span> list1<br>
<span>-</span> list2
~~~
<ul class="listClass">
  <li>list1</li>
  <li>list2</li>
</ul>
~~~
{{< /flexblock >}}
{ .flexblock }
