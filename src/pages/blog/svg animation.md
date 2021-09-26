---
templateKey: "blog-post"
title: "SVG animation in CSS"
date: 2021-09-02
featuredpost: false
featuredimage: /img/Node.js_logo.png
description: >-
  How to animate single and multiple layered SVG in CSS
tags:
  - css
  - svg
  - animation
---

Today we will animate two types of SVG
<br>

<!--
Our <b>single layered svg animation</b> will look like this -->

## Single layer animation

The <b>first</b> animation we will do is tħis <b> single layered </b> one

<iframe id="serviceFrameSend" src="https://asli-web.github.io/websites/" width="100%" height="250"  frameborder="0"></iframe>

<br>

## Setup

To start we will first need a SVG file.

<a href="/img/heart.svg" download style="width: 30px;">	
<svg style="margin: 10px; left:30px "
   xmlns:dc="http://purl.org/dc/elements/1.1/"
   xmlns:cc="http://creativecommons.org/ns#"
   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
   xmlns:svg="http://www.w3.org/2000/svg"
   xmlns="http://www.w3.org/2000/svg"
   xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"
   xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"
   width="60"
   height="60"
   id="svg2"
   version="1.1"
   inkscape:version="0.48.4 r9939"
   sodipodi:docname="Novo documento 1">
<defs
     id="defs4" />
<sodipodi:namedview
id="base"
pagecolor="#ffffff"
bordercolor="#666666"
borderopacity="1.0"
inkscape:pageopacity="0.0"
inkscape:pageshadow="2"
inkscape:zoom="5.3332631"
inkscape:cx="25.622065"
inkscape:cy="33.052464"
inkscape:document-units="px"
inkscape:current-layer="layer1"
showgrid="true"
borderlayer="true"
inkscape:showpageshadow="false"
inkscape:snap-bbox="true"
inkscape:window-width="1366"
inkscape:window-height="692"
inkscape:window-x="0"
inkscape:window-y="24"
inkscape:window-maximized="1">
<inkscape:grid
type="xygrid"
id="grid2985"
empspacing="2"
visible="true"
enabled="true"
snapvisiblegridlinesonly="true"
spacingx="6px"
spacingy="6px"
dotted="true" />
</sodipodi:namedview>
<metadata
     id="metadata7">
<rdf:RDF>
<cc:Work
rdf:about="">
<dc:format>image/svg+xml</dc:format>
<dc:type
rdf:resource="http://purl.org/dc/dcmitype/StillImage" />
<dc:title></dc:title>
</cc:Work>
</rdf:RDF>
</metadata>
<g
     inkscape:label="Camada 1"
     inkscape:groupmode="layer"
     id="layer1"
     transform="translate(0,-992.36218)">
<rect
       style="fill:#ffffff;fill-opacity:1;stroke:none"
       id="rect2987"
       width="6"
       height="6"
       x="12"
       y="1010.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950"
       width="6"
       height="6"
       x="18"
       y="998.36218" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-2"
       width="6"
       height="6"
       x="12"
       y="998.36218" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-6"
       width="6"
       height="6"
       x="24"
       y="1004.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-0"
       width="6"
       height="6"
       x="30"
       y="1004.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-23"
       width="6"
       height="6"
       x="36"
       y="998.36218" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-7"
       width="6"
       height="6"
       x="42"
       y="998.36218" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-07"
       width="6"
       height="6"
       x="48"
       y="998.36218" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-62"
       width="6"
       height="6"
       x="54"
       y="1004.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-5"
       width="6"
       height="6"
       x="54"
       y="1010.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-9"
       width="6"
       height="6"
       x="6"
       y="998.36218" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-57"
       width="6"
       height="6"
       x="1.7763568e-15"
       y="1004.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-1"
       width="6"
       height="6"
       x="1.7763568e-15"
       y="1010.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-28"
       width="6"
       height="6"
       x="1.7763568e-15"
       y="1016.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-72"
       width="6"
       height="6"
       x="54"
       y="1016.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-66"
       width="6"
       height="6"
       x="6"
       y="1022.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-00"
       width="6"
       height="6"
       x="12"
       y="1028.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-3"
       width="6"
       height="6"
       x="18"
       y="1034.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-99"
       width="6"
       height="6"
       x="24"
       y="1040.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-10"
       width="6"
       height="6"
       x="30"
       y="1040.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-38"
       width="6"
       height="6"
       x="36"
       y="1034.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-8"
       width="6"
       height="6"
       x="42"
       y="1028.3622" />
<rect
       style="fill:#000000;fill-opacity:1;stroke:none"
       id="rect3950-74"
       width="6"
       height="6"
       x="48"
       y="1022.3622" />
<rect
       style="fill:#9d0000;fill-opacity:1;stroke:none"
       id="rect3950-89"
       width="6"
       height="6"
       x="6"
       y="1004.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-7"
       width="6"
       height="6"
       x="12"
       y="1004.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-8"
       width="6"
       height="6"
       x="18"
       y="1004.3622" />
<rect
       style="fill:#9d0000;fill-opacity:1;stroke:none"
       id="rect3950-89-1"
       width="6"
       height="6"
       x="6"
       y="1010.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-76"
       width="6"
       height="6"
       x="12"
       y="1010.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-4"
       width="6"
       height="6"
       x="18"
       y="1010.3622" />
<rect
       style="fill:#9d0000;fill-opacity:1;stroke:none"
       id="rect3950-89-2"
       width="6"
       height="6"
       x="6"
       y="1016.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-79"
       width="6"
       height="6"
       x="12"
       y="1016.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-18"
       width="6"
       height="6"
       x="18"
       y="1016.3622" />
<rect
       style="fill:#9d0000;fill-opacity:1;stroke:none"
       id="rect3950-89-3"
       width="6"
       height="6"
       x="12"
       y="1022.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-0"
       width="6"
       height="6"
       x="18"
       y="1022.3622" />
<rect
       style="fill:#9d0000;fill-opacity:1;stroke:none"
       id="rect3950-89-5"
       width="6"
       height="6"
       x="18"
       y="1028.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-58"
       width="6"
       height="6"
       x="24"
       y="1028.3622" />
<rect
       style="fill:#9d0000;fill-opacity:1;stroke:none"
       id="rect3950-89-36"
       width="6"
       height="6"
       x="24"
       y="1034.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-09"
       width="6"
       height="6"
       x="30"
       y="1034.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-50"
       width="6"
       height="6"
       x="30"
       y="1028.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-27"
       width="6"
       height="6"
       x="24"
       y="1022.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-505"
       width="6"
       height="6"
       x="30"
       y="1022.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-24"
       width="6"
       height="6"
       x="30"
       y="1016.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-6"
       width="6"
       height="6"
       x="24"
       y="1016.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-12"
       width="6"
       height="6"
       x="24"
       y="1010.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-65"
       width="6"
       height="6"
       x="30"
       y="1010.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-9"
       width="6"
       height="6"
       x="36"
       y="1016.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-21"
       width="6"
       height="6"
       x="42"
       y="1022.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-39"
       width="6"
       height="6"
       x="36"
       y="1022.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-26"
       width="6"
       height="6"
       x="36"
       y="1028.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-95"
       width="6"
       height="6"
       x="42"
       y="1016.3622" />
<rect
       style="fill:#ff5757;fill-opacity:1;stroke:none"
       id="rect3950-89-86"
       width="6"
       height="6"
       x="48"
       y="1016.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-19"
       width="6"
       height="6"
       x="36"
       y="1010.3622" />
<rect
       style="fill:#ff0000;fill-opacity:1;stroke:none"
       id="rect3950-89-99"
       width="6"
       height="6"
       x="42"
       y="1010.3622" />
<rect
       style="fill:#ff5757;fill-opacity:1;stroke:none"
       id="rect3950-89-90"
       width="6"
       height="6"
       x="48"
       y="1010.3622" />
<rect
       style="fill:#ff5757;fill-opacity:1;stroke:none"
       id="rect3950-89-41"
       width="6"
       height="6"
       x="48"
       y="1004.3622" />
<rect
       style="fill:#ff5757;fill-opacity:1;stroke:none"
       id="rect3950-89-33"
       width="6"
       height="6"
       x="42"
       y="1004.3622" />
<rect
       style="fill:#ff5757;fill-opacity:1;stroke:none"
       id="rect3950-89-63"
       width="6"
       height="6"
       x="36"
       y="1004.3622" />
</g>
</svg>

</a>

(click to download)
<br><br>

Next we will add our SVG inside the body of our <b>HTML</b> file <b> 4 times </b>

```html
<body>
	<div class="hearts">
		<!-- shortened code -->
		<svg ...></svg>
		<svg ...></svg>
		<svg ...></svg>
		<svg ...></svg>
	</div>
</body>
```

<br>

## Animation

Now we will go to our <b>styles.css</b> and add our styling and animation.

Our <b>basic styling</b> looks like this:

```css
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
body {
	width: 100%;
	height: 100%;
}
.hearts {
	margin: auto;
	width: fit-content;
	height: 100%;
	position: relative;
}
svg {
	bottom: 0%;
	position: absolute;
}
```

<br>
To <b>animate</b> our hearts, we will now grab each one seperately and add <b>keyframes</b> to them
<br>

```css
svg:nth-child(1) {
	animation: ease-out heart 4s infinite;
}
svg:nth-child(2) {
	left: 10px;
	animation: ease-in-out heart2 3s infinite;
}
svg:nth-child(3) {
	left: 30px;
	animation: ease-in heart3 3.5s infinite;
}
svg:nth-child(4) {
	left: 53px;
	animation: heart4 2.8s infinite;
}
@keyframes heart {
	0% {
		transform: translate(0);
	}
	96% {
		transform: translateY(-800%);
		opacity: 1;
	}
	100% {
		transform: translateY(-800%);
		opacity: 0.4;
	}
}
@keyframes heart2 {
	0% {
		transform: translate(0);
	}
	96% {
		transform: translateY(-600%);
		opacity: 1;
	}
	100% {
		transform: translateY(-600%);
		opacity: 0.4;
	}
}
@keyframes heart3 {
	0% {
		transform: translate(0);
	}
	96% {
		transform: translateY(-680%);
		opacity: 1;
	}
	100% {
		transform: translateY(-680%);
		opacity: 0.4;
	}
}
@keyframes heart4 {
	0% {
		transform: translate(0);
	}
	96% {
		transform: translateY(-740%);
		opacity: 1;
	}
	100% {
		transform: translateY(-740%);
		opacity: 0.4;
	}
}
```

<br>
and that's it for our first animation.
<br>

## Multi layer animation

Our next animation will be a multi layered one.
<br>
We will grab certain parts of our SVG file and animate them.

<iframe id="serviceFrameSend" src="https://asli-web.github.io/anim/" width="100%" height="400"  frameborder="0"></iframe>

<br>

## Setup

First of all we will need a SVG file. <br>

If you haven't already have one, that you want to animate, then you might want to download one from a platform like <b>[iconscout](https://iconscout.com/)</b>.
<br><br>

Next we will open our SVG in a editor like <b>[Figma](https://www.figma.com/)</b>.
<br>
When we open our SVG, we will see many vectors, that represent different parts of our image.

![vectors](/img/vector.png "vector")
<br>
To make things easy, we can <b>rename</b> the vectors, that we later want to animate. <br><br>
Then we will save our File with an <b>ID</b> for each vector.

![id](/img/id.png "ID")

After that our SVG is ready to be used.<br><br>

### Animation

We will again import our SVG into the body of our <b>HTML file</b>, but this time every part of our SVG has an ID.

<br>
Then in our <b>styles.css</b>, we will beginn to animate our SVG. <br>
Our basic styling will look like this:

```css
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
body {
	width: 100%;
	height: 100%;
}

svg {
	width: 400px;
	height: max-content;
}
```

<br>

And our keyframes look like this:

```css
#bird {
	animation: moveBird 1.2s infinite alternate;
	transform-origin: bottom;
	transform-box: fill-box;
}
@keyframes moveBird {
	from {
		transform: rotate(0deg);
	}
	to {
		transform: rotate(6deg);
	}
}
#shoe {
	animation: moveShoe 0.7s infinite;
	transform-origin: start;
	transform-box: fill-box;
	transform: translate(-30px, -10px);
}
@keyframes moveShoe {
	from {
		transform: rotate(-0deg);
	}
	50% {
		transform: rotate(-3deg);
	}
	to {
		transform: rotate(3deg);
	}
}
```

<br>

And with that we finished our animation.
