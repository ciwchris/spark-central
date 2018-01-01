
<link rel="stylesheet" href="tufte.css"/>
<style>
body {
    padding-left: 0 !important;
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
        <svg width="400" height="50">
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
&lt;line x1="240" y1="15" x2="180" y2="35" stroke="paleturquoise"
    stroke-width="20" stroke-linecap="square" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="50">
            <line x1="50" y1="30" x2="350" y2="20" stroke="slateblue"
                stroke-width="10" stroke-linecap="round" />
            <line x1="210" y1="15" x2="190" y2="35" stroke="paleturquoise"
                stroke-width="20" stroke-linecap="square" />
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
        <svg width="400" height="50">
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
        <svg width="400" height="50">
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
        <svg width="400" height="50">
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
        <svg width="400" height="50">
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
        <svg width="400" height="100">
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
        <svg width="400" height="50">
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
        <svg width="400" height="120">
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
        <svg width="400" height="50">
            <text x="20" y="40" font-size="45"
                textLength="300" rotate="5"
                fill="transparent" stroke="plum" stroke-width="2">
                Let it snow!
            </text>
        </svg>
    </div>
</div>

[Transform](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/transform)
-----------

translate

<div class="content">
    <div>
        <pre>
            &lt;rect x="100" y="30" width="60" height="40"
                fill="pink" /&gt;
            &lt;rect x="100" y="30" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(10 10)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <rect x="100" y="30" width="60" height="40"
                fill="pink" />
            <rect x="100" y="30" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(10 10)" />
        </svg>
    </div>
</div>

Scale, but have to adjust position

<div class="content">
    <div>
        <pre>
            &lt;rect x="100" y="30" width="60" height="40"
                fill="pink" /&gt;
            &lt;rect x="55" y="20" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="scale(2 2)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <rect x="100" y="30" width="60" height="40"
                fill="pink" />
            <rect x="55" y="20" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="scale(2 2)" />
        </svg>
    </div>
</div>

Use translate and scale so you don't have to adjust

<div class="content">
    <div>
        <pre>
            &lt;rect x="100" y="30" width="60" height="40"
                fill="pink" /&gt;
            &lt;rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(110 40) scale(2 2)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <rect x="100" y="30" width="60" height="40"
                fill="pink" />
            <rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(110 40) scale(2 2)" />
        </svg>
    </div>
</div>

rotate

<div class="content">
    <div>
        <pre>
            &lt;rect x="100" y="30" width="60" height="40"
                fill="pink" /&gt;
            &lt;rect x="100" y="30" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="rotate(45 100 30)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <rect x="100" y="30" width="60" height="40"
                fill="pink" />
            <rect x="100" y="30" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="rotate(45 100 30)" />
        </svg>
    </div>
</div>

skewX skewY

<div class="content">
    <div>
        <pre>
            &lt;rect x="10" y="10" width="60" height="40"
                fill="pink" /&gt;
            &lt;rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(20 20) skewX(10)" /&gt;

            &lt;rect x="100" y="10" width="60" height="40"
                fill="pink" /&gt;
            &lt;rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(110 20) skewY(10)" /&gt;

            &lt;rect x="200" y="10" width="60" height="40"
                fill="pink" /&gt;
            &lt;rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(210 20) skewX(10) skewY(10)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <rect x="10" y="10" width="60" height="40"
                fill="pink" />
            <rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(20 20) skewX(10)" />

            <rect x="100" y="10" width="60" height="40"
            fill="pink" />
            <rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(110 20) skewY(10)" />

            <rect x="200" y="10" width="60" height="40"
                fill="pink" />
            <rect x="0" y="0" width="60" height="40"
                fill="mediumvioletred" fill-opacity=".8"
                transform="translate(210 20) skewX(10) skewY(10)" />
        </svg>
    </div>
</div>


[Animation](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/animateTransform)
-----------

Animate property: width

<div class="content">
    <div>
        <pre>
          &lt;rect x="100" y="10" width="100" height="50" fill="aliceblue" &gt;
            &lt;animate 
              attributeName="width"
              from="100" to="150"
              dur="3s"
              repeatCount="indefinite" /&gt;
          &lt;/rect&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
          <rect x="100" y="10" width="100" height="50" fill="aliceblue" >
            <animate 
              attributeName="width"
              from="100" to="150"
              dur="3s"
              repeatCount="indefinite" />
          </rect>
        </svg>
    </div>
</div>

Multiple animation properties

<div class="content">
    <div>
        <pre>
          &lt;rect x="100" y="10" width="100" height="50" fill="aliceblue" &gt;
            &lt;animate 
              attributeName="width"
              from="150" to="0"
              dur="3s"
              repeatCount="indefinite" /&gt;
            &lt;animate 
              attributeName="height"
              from="0" to="50"
              dur="3s"
              repeatCount="indefinite" /&gt;
          &lt;/rect&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
          <rect x="100" y="10" width="100" height="50" fill="aliceblue" >
            <animate 
              attributeName="width"
              from="150" to="0"
              dur="3s"
              repeatCount="indefinite" />
            <animate 
              attributeName="height"
              from="0" to="50"
              dur="3s"
              repeatCount="indefinite" />
          </rect>
        </svg>
    </div>
</div>

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
        <svg width="400" height="50">
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


Rotate:

<div class="content">
    <div>
        <pre>
            &lt;rect x="100" y="30" width="60" height="40" fill="indigo"&gt;
                &lt;animateTransform attributeName="transform"
                    type="rotate"
                    dur="10s"
                    from="0 130 50"
                    to="360 130 50"
                    repeatCount="indefinite" /&gt;
            &lt;/rect&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <rect x="100" y="30" width="60" height="40" fill="indigo">
                <animateTransform attributeName="transform"
                    type="rotate"
                    dur="10s"
                    from="0 130 50"
                    to="360 130 50"
                    repeatCount="indefinite" />
            </rect>
        </svg>
    </div>
</div>

Scale:

<div class="content">
    <div>
        <pre>
            &lt;circle cx="0" cy="0" r="20" fill="deeppink" transform="translate(100 50)"&gt;
                &lt;animateTransform attributeName="transform"
                    type="scale"
                    additive="sum"
                    dur="3s"
                    from=".5 .5"
                    to="2 2"
                    repeatCount="indefinite" /&gt;
            &lt;/circle&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <circle cx="0" cy="0" r="20" fill="deeppink" transform="translate(100 50)">
                <animateTransform attributeName="transform"
                    type="scale"
                    additive="sum"
                    dur="3s"
                    from=".5 .5"
                    to="2 2"
                    repeatCount="indefinite" />
            </circle>
        </svg>
    </div>
</div>


[Polygon](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/polygon)
---------

Straight lines

<div class="content">
    <div>
        <pre>
            &lt;polygon
                points="100 20 200 90 300 50 200 0"
                fill="orange" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <polygon
                points="100 20 200 90 300 50 200 0"
                fill="orange" />
        </svg>
    </div>
</div>

Complex

<div class="content">
    <div>
        <pre>
            &lt;polygon
                points="100 50 130 100 180 60 220 80 300 50 220 20 180 40 130 0"
                fill="paleturquoise" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <polygon
                points="100 50 130 100 180 60 220 80 300 50 220 20 180 40 130 0"
                fill="paleturquoise" />
        </svg>
    </div>
</div>

Combine with transform

<div class="content">
    <div>
        <pre>
            &lt;polygon
                points="0 50 30 100 80 60 120 80 200 50 120 20 80 40 30 0"
                fill="paleturquoise"
                transform="translate(200 0) rotate(90)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="200" >
            <polygon
                points="0 50 30 100 80 60 120 80 200 50 120 20 80 40 30 0"
                fill="paleturquoise"
                transform="translate(200 0) rotate(90)" />
        </svg>
    </div>
</div>



Gradients
---------

### [Linear](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/linearGradient) ###

Offset: where it stops being a pure color. So 98% is the transition area.

<div class="content">
    <div>
        <pre>
            &lt;defs&gt;
                &lt;linearGradient id="NoBlur"&gt;
                    &lt;stop offset="50%" stop-color="darkblue"/&gt;
                    &lt;stop offset="50%" stop-color="deepskyblue"/&gt;
                &lt;/linearGradient&gt;
                &lt;linearGradient id="Blur"&gt;
                    &lt;stop offset="0%" stop-color="darkblue"/&gt;
                    &lt;stop offset="100%" stop-color="deepskyblue"/&gt;
                &lt;/linearGradient&gt;
                &lt;linearGradient id="MultiBlur"&gt;
                    &lt;stop offset="0%" stop-color="darkblue"/&gt;
                    &lt;stop offset="50%" stop-color="dodgerblue"/&gt;
                    &lt;stop offset="100%" stop-color="deepskyblue"/&gt;
                &lt;/linearGradient&gt;
            &lt;/defs&gt;

            &lt;rect x="0" y="0" width="150" height="100"
                fill="url(#NoBlur)"/&gt;
            &lt;rect x="150" y="0" width="150" height="100"
                fill="url(#Blur)"/&gt;
            &lt;rect x="300" y="0" width="150" height="100"
                fill="url(#MultiBlur)"/&gt;
        </pre>
    </div>
    <div>
        <svg width="450" height="100" >
            <defs>
                <linearGradient id="NoBlur">
                    <stop offset="50%" stop-color="darkblue"/>
                    <stop offset="50%" stop-color="deepskyblue"/>
                </linearGradient>
                <linearGradient id="Blur">
                    <stop offset="0%" stop-color="darkblue"/>
                    <stop offset="100%" stop-color="deepskyblue"/>
                </linearGradient>
                <linearGradient id="MultiBlur">
                    <stop offset="0%" stop-color="darkblue"/>
                    <stop offset="50%" stop-color="dodgerblue"/>
                    <stop offset="100%" stop-color="deepskyblue"/>
                </linearGradient>
            </defs>

            <rect x="0" y="0" width="150" height="100"
                fill="url(#NoBlur)"/>
            <rect x="150" y="0" width="150" height="100"
                fill="url(#Blur)"/>
            <rect x="300" y="0" width="150" height="100"
                fill="url(#MultiBlur)"/>
        </svg>
    </div>
</div>

Can't reuse ids

<div class="content">
    <div>
        <pre>
            &lt;defs&gt;
                &lt;linearGradient id="CornerBlur" x1="0" y1="0" x2="1" y2="1"&gt;
                    &lt;stop offset="0%" stop-color="darkblue"/&gt;
                    &lt;stop offset="100%" stop-color="deepskyblue"/&gt;
                &lt;/linearGradient&gt;
                &lt;linearGradient id="CornerBlurReverse" x1="0" y1="1" x2="1" y2=".5"&gt;
                    &lt;stop offset="0%" stop-color="deepskyblue"/&gt;
                    &lt;stop offset="100%" stop-color="darkblue"/&gt;
                &lt;/linearGradient&gt;
            &lt;/defs&gt;

            &lt;rect x="0" y="0" width="200" height="100"
                fill="url(#CornerBlur)"/&gt;
            &lt;rect x="200" y="0" width="200" height="100"
                fill="url(#CornerBlurReverse)"/&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <defs>
                <linearGradient id="CornerBlur" x1="0" y1="0" x2="1" y2="1">
                    <stop offset="0%" stop-color="darkblue"/>
                    <stop offset="100%" stop-color="deepskyblue"/>
                </linearGradient>
                <linearGradient id="CornerBlurReverse" x1="0" y1="1" x2="1" y2=".5">
                    <stop offset="0%" stop-color="deepskyblue"/>
                    <stop offset="100%" stop-color="darkblue"/>
                </linearGradient>
            </defs>

            <rect x="0" y="0" width="200" height="100"
                fill="url(#CornerBlur)"/>
            <rect x="200" y="0" width="200" height="100"
                fill="url(#CornerBlurReverse)"/>
        </svg>
    </div>
</div>

### [Radial](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/radialGradient) ###

same

<div class="content">
    <div>
        <pre>
            &lt;defs&gt;
                &lt;radialGradient id="RadialGradient1"&gt;
                    &lt;stop offset="0%" stop-color="orchid"/&gt;
                    &lt;stop offset="100%" stop-color="mediumorchid"/&gt;
                &lt;/radialGradient&gt;
                &lt;radialGradient id="RadialGradient2"&gt;
                    &lt;stop offset="0%" stop-color="violet"/&gt;
                    &lt;stop offset="50%" stop-color="orchid" /&gt;
                    &lt;stop offset="100%" stop-color="mediumorchid"/&gt;
                &lt;/radialGradient&gt;
                &lt;radialGradient id="RadialGradient3"&gt;
                    &lt;stop offset="0%" stop-color="violet" stop-opacity=".8"/&gt;
                    &lt;stop offset="50%" stop-color="orchid" stop-opacity=".9"/&gt;
                    &lt;stop offset="100%" stop-color="mediumorchid" stop-opacity=".95"/&gt;
                &lt;/radialGradient&gt;
            &lt;/defs&gt;

            &lt;circle cx="50" cy="50" r="40"
                fill="url(#RadialGradient1)" /&gt;
            &lt;circle cx="150" cy="50" r="40"
                fill="url(#RadialGradient2)" /&gt;
            &lt;circle cx="250" cy="50" r="40"
                fill="url(#RadialGradient3)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="100" >
            <defs>
                <radialGradient id="RadialGradient1">
                    <stop offset="0%" stop-color="orchid"/>
                    <stop offset="100%" stop-color="mediumorchid"/>
                </radialGradient>
                <radialGradient id="RadialGradient2">
                    <stop offset="0%" stop-color="violet"/>
                    <stop offset="50%" stop-color="orchid" />
                    <stop offset="100%" stop-color="mediumorchid"/>
                </radialGradient>
                <radialGradient id="RadialGradient3">
                    <stop offset="0%" stop-color="violet" stop-opacity=".8"/>
                    <stop offset="50%" stop-color="orchid" stop-opacity=".9"/>
                    <stop offset="100%" stop-color="mediumorchid" stop-opacity=".95"/>
                </radialGradient>
            </defs>

            <circle cx="50" cy="50" r="40"
                fill="url(#RadialGradient1)" />
            <circle cx="150" cy="50" r="40"
                fill="url(#RadialGradient2)" />
            <circle cx="250" cy="50" r="40"
                fill="url(#RadialGradient3)" />
        </svg>
    </div>
</div>

Change location of

<div class="content">
    <div>
        <pre>
            &lt;defs&gt;
                &lt;radialGradient id="Gradient1" r=".3"&gt;
                    &lt;stop offset="10%" stop-color="orangered"/&gt;
                    &lt;stop offset="100%" stop-color="lightgoldenrodyellow"/&gt;
                &lt;/radialGradient&gt;
                &lt;radialGradient id="Gradient2" r=".3" cx=".3" cy=".7"&gt;
                    &lt;stop offset="10%" stop-color="orangered"/&gt;
                    &lt;stop offset="100%" stop-color="lightgoldenrodyellow"/&gt;
                &lt;/radialGradient&gt;
                &lt;radialGradient id="Gradient3" r=".3" cx=".3" cy=".7" fx=".35" fy=".6"&gt;
                    &lt;stop offset="10%" stop-color="orangered"/&gt;
                    &lt;stop offset="100%" stop-color="lightgoldenrodyellow"/&gt;
                &lt;/radialGradient&gt;
            &lt;/defs&gt;

            &lt;rect x="0" y="0" width="100" height="100"
                fill="url(#Gradient1)" /&gt;
            &lt;rect x="100" y="0" width="100" height="100"
                fill="url(#Gradient2)" /&gt;
            &lt;rect x="200" y="0" width="100" height="100"
                fill="url(#Gradient3)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="300" height="100" >
            <defs>
                <radialGradient id="Gradient1" r=".3">
                    <stop offset="10%" stop-color="orangered"/>
                    <stop offset="100%" stop-color="lightgoldenrodyellow"/>
                </radialGradient>
                <radialGradient id="Gradient2" r=".3" cx=".3" cy=".7">
                    <stop offset="10%" stop-color="orangered"/>
                    <stop offset="100%" stop-color="lightgoldenrodyellow"/>
                </radialGradient>
                <radialGradient id="Gradient3" r=".3" cx=".3" cy=".7" fx=".35" fy=".6">
                    <stop offset="10%" stop-color="orangered"/>
                    <stop offset="100%" stop-color="lightgoldenrodyellow"/>
                </radialGradient>
            </defs>

            <rect x="0" y="0" width="100" height="100"
                fill="url(#Gradient1)" />
            <rect x="100" y="0" width="100" height="100"
                fill="url(#Gradient2)" />
            <rect x="200" y="0" width="100" height="100"
                fill="url(#Gradient3)" />
        </svg>
    </div>
</div>

Animation with gradient

<div class="content">
    <div>
        <pre>
            &lt;defs&gt;
                &lt;radialGradient id="AnimatedGradient"&gt;
                    &lt;stop offset="1%" stop-color="hotpink"/&gt;
                    &lt;stop offset="99%" stop-color="deeppink"/&gt;
                &lt;/radialGradient&gt;
            &lt;/defs&gt;

            &lt;circle fill="url(#AnimatedGradient)" cx="0" cy="0" r="30" transform="translate(100 75)"&gt;
                &lt;animateTransform attributeName="transform"
                    type="scale"
                    additive="sum"
                    dur="3s"
                    from=".5 .5"
                    to="2 2"
                    repeatCount="indefinite" /&gt;
            &lt;/circle&gt;
        </pre>
    </div>
    <div>
        <svg width="200" height="150" >
            <defs>
                <radialGradient id="AnimatedGradient">
                    <stop offset="1%" stop-color="hotpink"/>
                    <stop offset="99%" stop-color="deeppink"/>
                </radialGradient>
            </defs>

            <circle fill="url(#AnimatedGradient)" cx="0" cy="0" r="30" transform="translate(100 75)">
                <animateTransform attributeName="transform"
                    type="scale"
                    additive="sum"
                    dur="3s"
                    from=".5 .5"
                    to="2 2"
                    repeatCount="indefinite" />
            </circle>
        </svg>
    </div>
</div>

Polygon with gradient

<div class="content">
    <div>
        <pre>
            &lt;defs&gt;
                &lt;radialGradient id="PolygonGradient" r=".7" cx=".2" &gt;
                    &lt;stop offset="1%" stop-color="paleturquoise"/&gt;
                    &lt;stop offset="99%" stop-color="deepskyblue"/&gt;
                &lt;/radialGradient&gt;
            &lt;/defs&gt;

            &lt;polygon
                points="0 50 30 100 80 60 120 80 200 50 120 20 80 40 30 0"
                fill="url(#PolygonGradient)"
                transform="translate(200 0) rotate(90)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="200" >
            <defs>
                <radialGradient id="PolygonGradient" r=".7" cx=".2" >
                    <stop offset="1%" stop-color="paleturquoise"/>
                    <stop offset="99%" stop-color="deepskyblue"/>
                </radialGradient>
            </defs>

            <polygon
                points="0 50 30 100 80 60 120 80 200 50 120 20 80 40 30 0"
                fill="url(#PolygonGradient)"
                transform="translate(200 0) rotate(90)" />
        </svg>
    </div>
</div>

[Filters](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/filter)
---------

SourceGraphic

<div class="content">
    <div>
        <pre>
            &lt;filter id="SameBlur"&gt;
                &lt;feGaussianBlur in="SourceGraphic" stdDeviation="5" /&gt;
            &lt;/filter&gt;
            &lt;filter id="DifferingBlur"&gt;
                &lt;feGaussianBlur in="SourceGraphic" stdDeviation="5 0" /&gt;
            &lt;/filter&gt;
            &lt;circle cx="50" cy="75" r="40" fill="springgreen"/&gt;
            &lt;circle cx="150" cy="75" r="40" fill="springgreen"
                filter="url(#SameBlur)"/&gt;
            &lt;circle cx="250" cy="75" r="40" fill="springgreen"
                filter="url(#DifferingBlur)"/&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="150" >
            <filter id="SameBlur">
                <feGaussianBlur in="SourceGraphic" stdDeviation="5" />
            </filter>
            <filter id="DifferingBlur">
                <feGaussianBlur in="SourceGraphic" stdDeviation="5 0" />
            </filter>
            <circle cx="50" cy="75" r="40" fill="springgreen"/>
            <circle cx="150" cy="75" r="40" fill="springgreen"
                filter="url(#SameBlur)"/>
            <circle cx="250" cy="75" r="40" fill="springgreen"
                filter="url(#DifferingBlur)"/>
        </svg>
    </div>
</div>

Drop shadow

<div class="content">
    <div>
        <pre>
            &lt;defs&gt;
                &lt;filter id="DropShadow" x="0" y="0" width="150%" height="150%"&gt;
                    &lt;feOffset result="offsetOut" in="SourceAlpha" dx="8" dy="8" /&gt;
                    &lt;feGaussianBlur result="blurOut" in="offsetOut" stdDeviation="6" /&gt;
                    &lt;feBlend in="SourceGraphic" in2="blurOut" mode="normal" /&gt;
                &lt;/filter&gt;
            &lt;/defs&gt;
 
            &lt;rect width="90" height="90" rx="5" ry="5"
                fill="darkcyan"
                filter="url(#DropShadow)" /&gt;
        </pre>
    </div>
    <div>
        <svg width="200" height="150">
            <defs>
                <filter id="DropShadow" x="0" y="0" width="150%" height="150%">
                    <feOffset result="offsetOut" in="SourceAlpha" dx="8" dy="8" />
                    <feGaussianBlur result="blurOut" in="offsetOut" stdDeviation="6" />
                    <feBlend in="SourceGraphic" in2="blurOut" mode="normal" />
                </filter>
            </defs>
 
            <rect width="90" height="90" rx="5" ry="5"
                fill="darkcyan"
                filter="url(#DropShadow)" />
       </svg> 
    </div>
</div>

[Groups](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/g) and [Use](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/use)
--------

Grouping

<div class="content">
    <div>
        <pre>
            &lt;g fill="gold" transform="rotate(25) translate(40 0)"&gt;
                &lt;circle cx="20" cy="15" r="8" /&gt;
                &lt;circle cx="37" cy="15" r="6" /&gt;
                &lt;circle cx="50" cy="15" r="4" /&gt;
                &lt;circle cx="60" cy="15" r="2" /&gt;
            &lt;/g&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="75">
            <g fill="gold" transform="rotate(25) translate(40 0)">
                <circle cx="20" cy="15" r="8" />
                <circle cx="37" cy="15" r="6" />
                <circle cx="50" cy="15" r="4" />
                <circle cx="60" cy="15" r="2" />
            </g>
        </svg>
    </div>
</div>

Using

<div class="content">
    <div>
        <pre>
            &lt;def&gt;
                &lt;g id="DotsTransformed" fill="gold"&gt;
                    &lt;circle r="8" /&gt;
                    &lt;circle r="6" transform="translate(17 0)" /&gt;
                    &lt;circle r="4" transform="translate(30 0)" /&gt;
                    &lt;circle r="2" transform="translate(40 0)" /&gt;
                &lt;/g&gt;
            &lt;/def&gt;
            &lt;use href="#DotsTransformed" transform="translate(50 20) rotate(20)"/&gt;
            &lt;use href="#DotsTransformed" transform="translate(140 20) rotate(160)"/&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="150">
            <def>
                <g id="DotsTransformed" fill="gold">
                    <circle r="8" />
                    <circle r="6" transform="translate(17 0)" />
                    <circle r="4" transform="translate(30 0)" />
                    <circle r="2" transform="translate(40 0)" />
                </g>
            </def>
            <use href="#DotsTransformed" transform="translate(50 20) rotate(20)"/>
            <use href="#DotsTransformed" transform="translate(140 20) rotate(160)"/>
        </svg>
    </div>
</div>


[Paths and Archs](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths)
-----------------

M: absolute move to
h: relative horizontal
v: relative vertical
Z: connect end to start

<div class="content">
    <div>
        <pre>
            &lt;path
                d="M10 10 h 80 v 80 h -80 Z"
                fill="transparent"
                stroke="royalblue" stroke-width="10"/&gt;
        </pre>
    </div>
    <div>
        <svg width="200" height="100">
            <path
                d="M10 10 h 80 v 80 h -80 Z"
                fill="transparent"
                stroke="royalblue" stroke-width="10"/>
        </svg>
    </div>
</div>

a: arch (a rx ry x-axis-rotation large-arc-flag sweep-flag dx dy)
two ellipses that can connect any two points
long either of those circles there are two possible paths that you can take to connect the points, so in any situation there are four possible arcs available.


<div class="content">
    <div>
        <pre>
            &lt;path
                d="M10 10 a 1 1 0 0 0 100 0"
                fill="cadetblue" stroke="cadetblue" /&gt;
            &lt;path
                d="M120 10 a 5 1 0 0 0 100 0"
                fill="lightseagreen" stroke="lightseagreen" /&gt;
            &lt;path
                d="M240 10 a 1 2 0 0 0 100 0"
                fill="mediumseagreen" stroke="mediumseagreen" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="150">
            <path
                d="M10 10 a 1 1 0 0 0 100 0"
                fill="cadetblue" stroke="cadetblue" />
            <path
                d="M120 10 a 5 1 0 0 0 100 0"
                fill="lightseagreen" stroke="lightseagreen" />
            <path
                d="M240 10 a 1 2 0 0 0 100 0"
                fill="mediumseagreen" stroke="mediumseagreen" />
        </svg>
    </div>
</div>

Set a different y ending position

<div class="content">
    <div>
        <pre>
            &lt;path
                d="M10 10 a 1 1 0 0 0 100 20"
                fill="fuchsia" stroke="fuchsia" /&gt;
            &lt;path
                d="M150 10 a 5 1 0 0 0 100 20"
                fill="deeppink" stroke="deeppink" /&gt;
            &lt;path
                d="M270 10 a 1 2 0 0 0 100 20"
                fill="mediumvioletred" stroke="mediumvioletred" /&gt;
        </pre>
    </div>
    <div>
        <svg width="400" height="150">
            <path
                d="M10 10 a 1 1 0 0 0 100 20"
                fill="fuchsia" stroke="fuchsia" />
            <path
                d="M150 10 a 5 1 0 0 0 100 20"
                fill="deeppink" stroke="deeppink" />
            <path
                d="M270 10 a 1 2 0 0 0 100 20"
                fill="mediumvioletred" stroke="mediumvioletred" />
        </svg>
    </div>
</div>


The third parameter describes the rotation of the arc

<div class="content">
    <div>
        <pre>
            &lt;path
                d="M30 0 a 2 1 0 0 0 100 0"
                fill="coral" stroke="coral" /&gt;
            &lt;path
                d="M150 0 a 2 1 22 0 0 100 0"
                fill="orange" stroke="orange" /&gt;
            &lt;path
                d="M280 0 a 2 1 45 0 0 100 0"
                fill="darkorange" stroke="darkorange" /&gt;
            &lt;path
                d="M410 0 a 2 1 57 0 0 100 0"
                fill="tomato" stroke="tomato" /&gt;
            &lt;path
                d="M540 0 a 2 1 90 0 0 100 0"
                fill="orangered" stroke="orangered" /&gt;
        </pre>
    </div>
    <div>
        <svg width="650" height="110">
            <path
                d="M30 0 a 2 1 0 0 0 100 0"
                fill="coral" stroke="coral" />
            <path
                d="M150 0 a 2 1 22 0 0 100 0"
                fill="orange" stroke="orange" />
            <path
                d="M280 0 a 2 1 45 0 0 100 0"
                fill="darkorange" stroke="darkorange" />
            <path
                d="M410 0 a 2 1 57 0 0 100 0"
                fill="tomato" stroke="tomato" />
            <path
                d="M540 0 a 2 1 90 0 0 100 0"
                fill="orangered" stroke="orangered" />
        </svg>
    </div>
</div>

The second argument is the sweep-flag. It determines if the arc should begin moving at positive angles or negative ones, which essentially picks which of the two circles you will travel around. 

It simply determines if the arc should be greater than or less than 180 degrees; in the end, this flag determines which direction the arc will travel around a given circle.

<div class="content">
    <div>
        <pre>
            &lt;path
                d="M10 110 a 60 60 0 0 0 100 0"
                fill="aqua" stroke="aqua" /&gt;
            &lt;path
                d="M120 110 a 60 60 0 0 1 100 0"
                fill="aquamarine" stroke="aquamarine" /&gt;
            &lt;path
                d="M230 110 a 60 60 0 1 0 100 0"
                fill="palegreen" stroke="palegreen" /&gt;
            &lt;path
                d="M340 110 a 60 60 0 1 1 100 0"
                fill="greenyellow" stroke="greenyellow" /&gt;
        </pre>
    </div>
    <div>
        <svg width="460" height="210">
            <path
                d="M10 110 a 60 60 0 0 0 100 0"
                fill="aqua" stroke="aqua" />
            <path
                d="M120 110 a 60 60 0 0 1 100 0"
                fill="aquamarine" stroke="aquamarine" />
            <path
                d="M230 110 a 60 60 0 1 0 100 0"
                fill="palegreen" stroke="palegreen" />
            <path
                d="M340 110 a 60 60 0 1 1 100 0"
                fill="greenyellow" stroke="greenyellow" />
        </svg>
    </div>
</div>


[View box](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/viewBox)
----------

Zooming


<div class="content">
    <div>
        <pre>
            &lt;svg width="150" height="150" viewBox="0 0 150 150"&gt;
                &lt;rect width="200%" height="200%" fill="lightsteelblue"/&gt;
                &lt;rect x="5" y="5" rx="5" ry="5"
                    width="75" height="75"
                    fill="springgreen"/&gt;
                &lt;circle cx="100" cy="100" r="25"
                    fill="greenyellow" /&gt;
            &lt;/svg&gt;
            &lt;svg width="150" height="150" viewBox="0 0 100 100" &gt;
                &lt;rect width="200%" height="200%" fill="lightsteelblue"/&gt;
                &lt;rect x="5" y="5" rx="5" ry="5"
                    width="75" height="75"
                    fill="springgreen"/&gt;
                &lt;circle cx="100" cy="100" r="25"
                    fill="greenyellow" /&gt;
            &lt;/svg&gt;
            &lt;svg width="150" height="150" viewBox="0 0 200 200" &gt;
                &lt;rect width="200%" height="200%" fill="lightsteelblue"/&gt;
                &lt;rect x="5" y="5" rx="5" ry="5"
                    width="75" height="75"
                    fill="springgreen"/&gt;
                &lt;circle cx="100" cy="100" r="25"
                    fill="greenyellow" /&gt;
            &lt;/svg&gt;
        </pre>
    </div>
    <div>
        <svg width="150" height="150" viewBox="0 0 150 150">
            <rect width="200%" height="200%" fill="lightsteelblue"/>
            <rect x="5" y="5" rx="5" ry="5"
                width="75" height="75"
                fill="springgreen"/>
            <circle cx="100" cy="100" r="25"
                fill="greenyellow" />
        </svg>
        <svg width="150" height="150" viewBox="0 0 100 100" >
            <rect width="200%" height="200%" fill="lightsteelblue"/>
            <rect x="5" y="5" rx="5" ry="5"
                width="75" height="75"
                fill="springgreen"/>
            <circle cx="100" cy="100" r="25"
                fill="greenyellow" />
        </svg>
        <svg width="150" height="150" viewBox="0 0 200 200" >
            <rect width="200%" height="200%" fill="lightsteelblue"/>
            <rect x="5" y="5" rx="5" ry="5"
                width="75" height="75"
                fill="springgreen"/>
            <circle cx="100" cy="100" r="25"
                fill="greenyellow" />
        </svg>
    </div>
</div>

Different starting

<div class="content">
    <div>
        <pre>
            &lt;svg width="150" height="150" viewBox="40 40 150 150"&gt;
                &lt;rect width="200%" height="200%" fill="lightsteelblue"/&gt;
                &lt;rect x="5" y="5" rx="5" ry="5"
                    width="75" height="75"
                    fill="springgreen"/&gt;
                &lt;circle cx="100" cy="100" r="25"
                    fill="greenyellow" /&gt;
            &lt;/svg&gt;
            &lt;svg width="150" height="150" viewBox="30 30 100 100" &gt;
                &lt;rect width="200%" height="200%" fill="lightsteelblue"/&gt;
                &lt;rect x="5" y="5" rx="5" ry="5"
                    width="75" height="75"
                    fill="springgreen" /&gt;
                &lt;circle cx="100" cy="100" r="25"
                    fill="greenyellow" /&gt;
            &lt;/svg&gt;
            &lt;svg width="150" height="150" viewBox="50 50 200 200" &gt;
                &lt;rect width="200%" height="200%" fill="lightsteelblue"/&gt;
                &lt;rect x="5" y="5" rx="5" ry="5"
                    width="75" height="75"
                    fill="springgreen"/&gt;
                &lt;circle cx="100" cy="100" r="25"
                    fill="greenyellow" /&gt;
            &lt;/svg&gt;
        </pre>
    </div>
    <div>
        <svg width="150" height="150" viewBox="40 40 150 150">
            <rect width="200%" height="200%" fill="lightsteelblue"/>
            <rect x="5" y="5" rx="5" ry="5"
                width="75" height="75"
                fill="springgreen"/>
            <circle cx="100" cy="100" r="25"
                fill="greenyellow" />
        </svg>
        <svg width="150" height="150" viewBox="30 30 100 100" >
            <rect width="200%" height="200%" fill="lightsteelblue"/>
            <rect x="5" y="5" rx="5" ry="5"
                width="75" height="75"
                fill="springgreen" />
            <circle cx="100" cy="100" r="25"
                fill="greenyellow" />
        </svg>
        <svg width="150" height="150" viewBox="50 50 200 200" >
            <rect width="200%" height="200%" fill="lightsteelblue"/>
            <rect x="5" y="5" rx="5" ry="5"
                width="75" height="75"
                fill="springgreen"/>
            <circle cx="100" cy="100" r="25"
                fill="greenyellow" />
        </svg>
    </div>
</div>
