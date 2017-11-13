
<link rel="stylesheet" href="tufte.css"/>
<style>
body {
    padding-left: 0;
}
.content {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    border: 3px dashed salmon;
    border-radius: 5px;
    padding: 10px;
}
pre {
    font-size: .8rem;
}
.code {
    background-color: beige;
    padding: 2px 6px;
}
</style>

[Lines](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/line)
-------

Draw lines from first point (x1, y1) to second point (x2, y2)

- Set the color of the line: <span class="code">[`stroke="green"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke)</span>
- Try different [color names](https://upload.wikimedia.org/wikipedia/commons/2/2b/SVG_Recognized_color_keyword_names.svg)

<div class="content">
    <div>
        <pre>
&lt;line x1="50" y1="10" x2="350" y2="40" stroke="green" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <line x1="50" y1="10" x2="350" y2="40" stroke="green" />
        </svg>
    </div>
</div>


Try including these other properties with lines:

- Line size: <span class="code">[`stroke-width="10"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke-width)</span>
- How line starts and ends (values: butt, round, square): <span class="code">[`stroke-linecap="round"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke-linecap)</span>
- Try drawing multiple lines

<div class="content">
    <div>
        <pre>
&lt;line x1="50" y1="30" x2="350" y2="20" stroke="slateblue"
    stroke-width="10" stroke-linecap="round" /&gt;
&lt;line x1="240" y1="10" x2="180" y2="40" stroke="paleturquoise"
    stroke-width="10" stroke-linecap="square" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <line x1="50" y1="30" x2="350" y2="20" stroke="slateblue"
                stroke-width="10" stroke-linecap="round" />
            <line x1="210" y1="10" x2="190" y2="40" stroke="paleturquoise"
                stroke-width="10" stroke-linecap="square" />
        </svg>
    </div>
</div>



[Rectangles](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/rect)
-----------

Draw rectangles from upper left point (x, y) with a width and height

<div class="content">
    <div>
        <pre>
&lt;rect x="5" y="5" width="390" height="40" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <rect x="5" y="5" width="390" height="40" />
        </svg>
    </div>
</div>

Try including these other attributes with rectangles:

- Round corners: <span class="code">`rx="5" ry="5"`</span>
- Color: <span class="code">[`fill="dimgray"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/fill)</span>
- Transparent: <span class="code">`fill="transparent"`</span>
- Border color and size: <span class="code">`stroke="orchid" stroke-width="5"`</span>
- Make it see through (values: 0.0-1.0): <span class="code">[`fill-opacity=".5"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/fill-opacity)</span>
- Also make borders see through (values: 0.0-1.0): <span class="code">[`opacity=".5"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/opacity)</span>

<div class="content">
    <div>
        <pre>
&lt;rect x="5" y="5" width="80" height="30"
    fill="orangered" rx="10" ry="10" /&gt;
&lt;rect x="110" y="2" width="80" height="45"
    fill="transparent" stroke="orchid" stroke-width="5" /&gt;

&lt;rect x="250" y="5" width="100" height="35"
    rx="20" ry="20" fill="seagreen"
    stroke="lightseagreen" stroke-width="5" /&gt;
&lt;rect x="220" y="20" width="60" height="30"
    fill="powderblue" fill-opacity=".5"
    stroke="royalblue" stroke-width="5" /&gt;
&lt;rect x="320" y="20" width="60" height="30"
    fill="powderblue" opacity=".5"
    stroke="royalblue" stroke-width="5" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <rect x="5" y="5" width="80" height="30"
                fill="orangered" rx="10" ry="10" />
            <rect x="110" y="2" width="80" height="45"
                fill="transparent" stroke="orchid" stroke-width="5" />

            <rect x="250" y="5" width="100" height="35"
                rx="20" ry="20" fill="seagreen"
                stroke="lightseagreen" stroke-width="5" />
            <rect x="220" y="20" width="60" height="30"
                fill="powderblue" fill-opacity=".5"
                stroke="royalblue" stroke-width="5" />
            <rect x="320" y="20" width="60" height="30"
                fill="powderblue" opacity=".5"
                stroke="royalblue" stroke-width="5" />
        </svg>
    </div>
</div>




[Circles](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/circle) & [Ellipses](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/ellipse)
---------

Draw circles at a point (cx, cy) with a radius

<div class="content">
    <div>
        <pre>
&lt;circle cx="200" cy="25" r="20" fill="yellow" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <circle cx="200" cy="25" r="20" fill="yellow" />
        </svg>
    </div>
</div>

Draw ellipses at a point (cx, cy) with a both a vertical and horizontal radius (rx, ry)

<div class="content">
    <div>
        <pre>
&lt;ellipse cx="200" cy="25" rx="50" ry="20" fill="greenyellow" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <ellipse cx="200" cy="25" rx="50" ry="20" fill="greenyellow" />
        </svg>
    </div>
</div>

Try using the other attributes you learned with rectangles

<div class="content">
    <div>
        <pre>
&lt;circle cx="200" cy="50" r="40"
    fill="transparent" stroke="lavender" stroke-width="3"/&gt;
&lt;ellipse cx="200" cy="50" rx="40" ry="15"
    fill="transparent" stroke="lavender" stroke-width="3"/&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" xmlns="http://www.w3.org/2000/svg">
            <circle cx="200" cy="50" r="40" stroke="lavender" fill="transparent" stroke-width="3"/>
            <ellipse cx="200" cy="50" rx="40" ry="15" stroke="lavender" fill="transparent" stroke-width="3"/>
        </svg>
    </div>
</div>


[Text](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/text)
------

Add text to images at the point (x, y)

<div class="content">
    <div>
        <pre>
&lt;text x="20" y="40" font-size="25" &gt;
    Let it snow, let it snow, let it snow!
&lt;/text&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <text x="20" y="40" font-size="25">
                Let it snow, let it snow, let it snow!
            </text>
        </svg>
    </div>
</div>

Try including these other attributes with text:

- Stretch text to a length: <span class="code">[`textLength="300"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/textLength)</span>
- Change how text stretches (values: spacing, spacingAndGlyphs): <span class="code">[`lengthAdjust="spacing"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/lengthAdjust)</span>
- Rotate the text: <span class="code">[`rotate="10"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/rotate)</span>

<div class="content">
    <div>
        <pre>
&lt;text x="0" y="20" font-size="25"
    textLength="300" lengthAdjust="spacing"&gt;
    Let it snow!
&lt;/text&gt;
&lt;text x="0" y="60" font-size="25"
    textLength="300" lengthAdjust="spacingAndGlyphs"&gt;
    Let it snow!
&lt;/text&gt;
&lt;text x="20" y="100" font-size="25"
    textLength="300" lengthAdjust="spacing"
    rotate="-90"&gt;
    Let it snow!
&lt;/text&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="120" xmlns="http://www.w3.org/2000/svg">
            <text x="0" y="20" font-size="25"
                textLength="300" lengthAdjust="spacing">
                Let it snow!
            </text>
            <text x="0" y="60" font-size="25"
                textLength="300" lengthAdjust="spacingAndGlyphs">
                Let it snow!
            </text>
            <text x="20" y="100" font-size="25"
                textLength="300" lengthAdjust="spacing"
                rotate="-90">
                Let it snow!
            </text>
        </svg>
    </div>
</div>

Try using the other attributes you've learned

<div class="content">
    <div>
        <pre>
&lt;text x="20" y="40" font-size="45"
    textLength="300" rotate="5"
    fill="transparent" stroke="plum" stroke-width="2"&gt;
    Let it snow!
&lt;/text&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <text x="20" y="40" font-size="45"
                textLength="300" rotate="5"
                fill="transparent" stroke="plum" stroke-width="2">
                Let it snow!
            </text>
        </svg>
    </div>
</div>

[Animation](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/animateTransform)
-----------

Move an item from one location to another and have the movement occur over a length of time.
The type of movement we will perform is called `translate`. We will tell the animation what
point to begin, `from`, where to end, `to` and the number of seconds, `dur`, for it to take.

- Begin: <span class="code">[`from="50 0"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/from)</span>
- End: <span class="code">[`to="200 0"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/to)</span>
- How long: <span class="code">[`dur="10s"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/dur)</span>
- How many times to perform the animation: <span class="code">[`repeatCount="indefinite"`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/repeatCount)</span>

<div class="content">
    <div>
        <pre>
&lt;circle cx="50" cy="25" r="20" fill="yellow"&gt;
    &lt;animateTransform attributeName="transform"
        type="translate"
        from="50 0"
        to="200 0"
        dur="10s"
        repeatCount="indefinite" /&gt;
&lt;/circle&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50" xmlns="http://www.w3.org/2000/svg">
            <circle cx="50" cy="25" r="20" fill="yellow">
                <animateTransform attributeName="transform"
                    type="translate"
                    from="50 0"
                    to="200 0"
                    dur="10s"
                    repeatCount="indefinite" />
            </circle>
        </svg>
    </div>
</div>

Polygon
-------

```
<polygon
    points="395 210 400 220 405 210"
    fill="orange" />
```

Gradients
---------

```
<linearGradient id="SkyGradient" x1="0" x2="0" y1="0" y2="1">
    <stop offset="5%" stop-color="darkblue"/>
    <stop offset="95%" stop-color="lightblue"/>
</linearGradient>
```

```
<rect x="4" y="4" width="793" height="400" fill="url(#SkyGradient)"/>
<rect x="4" y="404" width="793" height="42" fill="floralwhite"/>
```

Filters
-------

```
<filter id="SunBlur">
    <feGaussianBlur in="SourceGraphic" stdDeviation="2" />
</filter>
<circle cx="150" cy="70" r="40" fill="yellow" filter="url(#SunBlur)"/>
```

Groups and Use
--------------

```
<g id="Pebble">
    <circle r="4" />
</g>
<g id="SmallPebble">
    <circle r="2" />
</g>
```


Paths and Archs
---------------

```
<path d="M-140 130
         a 25 25, 0, 0, 0, 40 0
         a 45 25, 0, 0, 0, 80 0
         a 20 25, 0, 1, 0, 0 -50
         a 45 25, 0, 0, 0, -120 0
         a 20 25, 0, 1, 0, 0 50
         Z" fill="floralwhite" opacity=".8" id="Cloud">
    <animateTransform attributeName="transform"
        type="translate"
        from="962 0"
        to="0 0"
        dur="50s"
        repeatCount="indefinite" />
</path>
```

View Box
--------

```
<svg preserveAspectRatio="xMidYMid slice" viewBox="0 0 801 450" xmlns="http://www.w3.org/2000/svg">
</svg>
```
