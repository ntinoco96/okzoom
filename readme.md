#okzoom#

##OKZoom by OKFocus##
OKZoom is a jQuery plugin that produces a portable loupe of variable size and shape. All other jQuery 'zoom' plugins we have encountered implement a square magnifying area. Ours is a circle. You want a circle. See a demo "here":http://okfoc.us/okzoom.

##Usage##
You can install OKZoom via npm: __npm install okzoom__ or download the source code

After installing or downloading the source code, you can bind OKZoom to one or many image elements, producing a "zoom" effect like this:

![image example](https://github.com/okfocus/okzoom/raw/master/demos/img/okshadow-example.png "Example Image")

With code like this:

```
$('img').okzoom({
  width: 200,
  height: 200,
  round: true,
  background: "#fff",
  backgroundRepeat: "repeat",
  shadow: "0 0 5px #000",
  border: "1px solid black"
});
```

###Options##

|Usage           |                                          |             |
|----------------|------------------------------------------|-------------|
|width           |(in pixels}                               |150          |
|height          |(in pixels}                               |150          |
|scaleWidth      |optionally resize the loupe image         |null         |
|round           |round loupe if true, square if false      |true         |
|background      |color for image off the edge of the loupe |#fff         |
|backgroundRepeat|repeat the image within the loupe         |no-repeat    |
|border          |border around the loupe                   |0            |
|shadow          |box-shadow on the loupe                   |0 0 5px #000 |

###Data Attribute###
Typically, we use this plugin on an image that has been sized down in HTML, and the loupe displays the image at its normal size.  If you like, you can add an HTML5 data attribute **data-okimage** to your image to substitute alternative content inside the loupe.

###Run Tests###

OKFocus tests JavaScript with Jasmine. Run tests:

```
$ bundle install
$ jasmine init
$ rake jasmine
```
