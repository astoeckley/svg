## What is it?

This [Elm](http://elm-lang.org) package builds on top of the
[opensolid/geometry](http://package.elm-lang.org/packages/opensolid/geometry/latest)
package to draw SVG diagrams in a flexible and expressive way. It contains
functions for drawing OpenSolid 2D geometric objects as SVG, and for applying
OpenSolid-based 2D transformations to arbitrary SVG elements.

## Drawing functions

The `lineSegment2d`, `triangle2d`, `polyline2d`, `polygon2d`, and `circle2d`
functions all produce standard
[Svg msg](http://package.elm-lang.org/packages/elm-lang/svg/latest/Svg#Svg)
values that can be included in any SVG diagram:

![lineSegment2d](https://opensolid.github.io/images/svg/1.0/lineSegment2d.svg)
![triangle2d](https://opensolid.github.io/images/svg/1.0/triangle2d.svg)
![polyline2d](https://opensolid.github.io/images/svg/1.0/polyline2d.svg)
![polygon2d](https://opensolid.github.io/images/svg/1.0/polygon2d.svg)
![circle2d](https://opensolid.github.io/images/svg/1.0/circle2d.svg)

The appearance of the resulting elements can be fully customized by adding SVG
attributes such as `fill` and `stroke`.

## Transformation functions

The `scaleAbout`, `rotateAround`, `translateBy`, `mirrorAcross`, `relativeTo`
and `placeIn` functions behave just like their standard OpenSolid counterparts.
You can use them to do things that would be difficult to do using just SVG, such
as mirror a fragment of SVG across an arbitrary axis:

![scaleAbout](https://opensolid.github.io/images/svg/1.0/scaleAbout.svg)
![rotateAround](https://opensolid.github.io/images/svg/1.0/rotateAround.svg)
![translateBy](https://opensolid.github.io/images/svg/1.0/translateBy.svg)
![mirrorAcross](https://opensolid.github.io/images/svg/1.0/mirrorAcross.svg)
![placeIn](https://opensolid.github.io/images/svg/1.0/placeIn.svg)

## Installation

Assuming you have [installed Elm](https://guide.elm-lang.org/install.html) and
started a new project, use [elm-package](https://guide.elm-lang.org/install.html#elm-package)
to install `opensolid/svg`, either by running

```
elm package install opensolid/svg
```

in a command prompt inside your project directory or by adding

```json
"opensolid/svg": "1.0.0 <= v < 2.0.0"
```

to your project's `elm-package.json`.

## Documentation

Full API documentation is available.