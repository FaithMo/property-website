## A Brief Overview of HTML5
- First released in **2014**, whike the first version of HTML was developed in **1993**.
- Its aim was to introduce sematintic elements. 
### Semantic Elements
Semantic elements describe their meaning to both developers and the browsers.

![semantic elements](/images/image.png)

- HTML5 refers to _2 things_:
  - It is an updated HTML language itself and contains new elements and attributes.
  - A larger set of technologies that work with the new version of HTML, such as **a new video format**, allowing you to create **more complex and powerful websites and applications**.
<br>
- HTML5 was designed in such a way as to eliminate the need for non-standard proprietary technologies,e.g. plugins, flash etc.
- This new version of HTML allows you to create web applications that work ***offline**, support **high-definition videos and animations**, and know where you are **geographically**. 

### Changes
- To make the code easier for users and screen readers to understand.
- Reducing **overlaps** between HTML, CSS, and Javascripts.
- Promoting **responsiveness** and and **design consistency** across browsers.
- **Multimedia support** without the use of Flash or any other plugins.

### Benefits of HTML5
1. **Semantic markup**: introduces elements that better describe the content of a web page. It makes it easy for the search engines to understand the content of a page and rank it higher in the search results.
2. **Improving cross-browser compatibility**: Designed to be more compatible withe different browsers. Websites are most likely going to look similar in all browsers.
3. **New APIs**: New apis such as < canvas > and < video >
4. **Mobile-friendliness**: Making websites that look and function well on mobile devices. 

<hr>

### New Semantic Elements 
All these make it easier to write cleaner code that clearly distinguishes style from content, which is particularly important for users using assistive technologies such as screen readers.

- section
  - A section element is similar to an article element. However, a section element can be used for content on a page that does not necessarily relate to other content on that page. For example, if you look at the home page of most websites, you will see different sections that stand alone and do not necessarily represent or have anything to do with the other sections on that page. Another example would be a news website where sections are broken down by topics such as sports news, travel news, current affairs, etc.
- header
  - provides introductory informartion for a page. contains heading/and navigational aids.
  - In addition to holding a < h1> or title, it can also hold a list of content for a page or an image. 
  - The header is used to define the heading of each section on a page, where you would use heading tags (**< h1> to < h6>**).
- footer
- nav
  - Is part of a page that **links** to other pages or sections. 
  - Often used in a content list to direct users to another part of a page. Similarly,it is often used as a page's **menu or index**.
- mark
- figure
- figcaption
- aside
- article
  - Used to show independent content (standalone content that sits on the page). For example, **it may be a blog post, an interactive widget, or even a user comment on an article.**
- data
- time
- output
- progress
- meter
- main

Blockquote
```markdown
< blockquote cite="https://www.techtarget.com">
<p>A paragraph of text goes here…</p>
< /blockquote>
```

### HTML Media Elements

#### Images

```
<img src="folder/imageexample.png" -- LOCATION
     alt="Image Description" -- IMAGE ATTRIBUTES
     width="150" 
     height="100"
     border="3" />
```

#### Videos

```
<video width="400" controls> 
    <source src="location/video.mp4 type="video/mp4" />
    Your browser does not support HTML video.
</video>

<p>

Video courtesy of <a href="https://www.google.com/" target="_blank">Video found online</a>.
</p>
```

#### Audio

```
<audio controls>

  <source src="https://www.learningcontainer.com/wp-content/uploads/2020/02/Kalimba.mp3" type="audio/mpeg">

Your browser does not support the audio element.

</audio>
```
<hr>

### Advances HTML Features

1. **Semantic Markup**: HTML5 introduces new semantic elements like `<header>, <footer>, <nav>, <article>, <section>, <aside>, <main>`, etc., which provide a clearer structure to web documents, aiding accessibility, SEO, and overall document organization.

2. **Canvas and SVG**: HTML5 offers two powerful graphics technologies - `<canvas>` and SVG (Scalable Vector Graphics). `<canvas>` allows dynamic rendering of graphics using JavaScript, while SVG provides resolution-independent vector graphics directly in HTML.

3. **Web Storage**: HTML5 provides two mechanisms for storing data on the client-side - localStorage and sessionStorage. These offer more storage capacity compared to cookies and are available for the entire duration of the page session or persist even after the browser is closed, respectively.

4. **Web Workers**: Web Workers enable concurrent execution of scripts in the background, allowing tasks to be performed without blocking the main UI thread. This helps improve performance and responsiveness in web applications, especially for computationally intensive tasks.

5. **Web Sockets**: Web Sockets facilitate real-time communication between the client and server over a single, long-lived connection. This enables bi-directional, low-latency communication, making it ideal for applications requiring instant updates or multiplayer gaming.

6. **Geolocation API**: HTML5's Geolocation API allows web applications to access the user's geographical location using JavaScript. This enables location-based services, such as mapping, local search, and targeted content delivery.

7. **Offline Web Applications**: HTML5 introduces features like the Application Cache (appcache) and Service Workers, enabling web applications to work offline or under unstable network conditions. This improves user experience and accessibility, particularly for mobile users.

8. **Audio and Video**: HTML5 provides native support for embedding audio and video content directly into web pages using the <audio> and <video> elements, eliminating the need for third-party plugins like Flash. This enhances compatibility, accessibility, and performance.

9. **Form Enhancements**: HTML5 introduces several new form input types (`<input type="date">, <input type="email">, <input type="tel">`, etc.) and attributes (required, placeholder, pattern, etc.), along with the `<datalist>` element for autocomplete functionality, making forms more user-friendly and accessible.

10. **Responsive Web Design**: While not exclusive to HTML5, the concept of responsive web design has gained prominence with the advent of HTML5 and CSS3. HTML5 features like semantic markup, media queries, and flexible layouts enable developers to create websites that adapt seamlessly to different devices and screen sizes.

#### 11. HTML Lists.
1. HTML offers **three** ways to display lists of imformation. 
2. All lists must contain one or more list elements. Lists may contain: `<ul>` − an **unordered** list. This will list items using plain bullets. You can use the type attribute for the `<ul>` tag to specify the type of bullet you like. By default, it is a disc. Following are the possible options, such as square, disc, and circle.
##### Unorded list
```
AN UNORDERED LIST - DEFAULT
<ul>
    <li>Beetroot</li>
    <li>Ginger</li>
    <li>Potato</li>
    <li>Radish</li>
</ul>

OUTPUT
- Beetroot
- Ginger
- Potato
- Radish

OR SQUARE TYPE 
<ul type="square">
    <li>Beetroot</li>
    <li>Ginger</li>
    <li>Potato</li>
    <li>Radish</li>
</ul>
```
##### Ordered list
`<ol>` is an ordered list. This will use different schemes of numbers to list your items. You can use the type attribute for the `<ol>` tag to specify the type of numbering you like. By default, it is a number. Following are the possible options: **default numerals, upper-case numerals, lower-case numerals, upper-case letters, and lower-case numerals**. Also, the start attribute for the `<ol>` tag may be used to specify the **starting point of numbering**.
```
<ol>
    <li>Beetroot</li>
    <li>Ginger</li>
    <li>Potato</li>
    <li>Radish</li>
</ol>

OUTPUT
1. Beetroot
2. Ginger
3. Potato
4. Radish

<ol type = "A">
    <li>Lion</li>
    <li>Tiger</li>
    <li>Mouse</li>
    <li>Horse</li>
</ol>

OUTPUT
A. Lion
B. Tiger
C. Mouse
D. Horse

<ol type = "1" start = "10">
    <li>Lion</li>
    <li>Tiger</li>
    <li>Mouse</li>
    <li>Horse</li>
</ol>

OUTPUT
10. Lion
11. Tiger
12. Mouse
13. Horse

```

#### `<dl>` − is a definition list

·`<dl>` − defines the start of the list, and `</dl>` − defines the end of the list.
·`<dt>` − a term
·`<dd>` − term definition

```
<dl>
    <dt><b>HTML</b></dt>
    <dd>This stands for Hyper Text Markup Language</dd>
    <dt><b>HTTP</b></dt>
    <dd>This stands for Hyper Text Transfer Protocol</dd>
  </dl>
  ```