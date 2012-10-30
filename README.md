Starling-Extension-Graphics
===========================

This extension adds a suite of graphics primitives such as Planes, Fills and Strokes. These are starling display objects that are automatically triangulated for fast rendering on the GPU.

These primitives can be manipulated directly, or created on your behalf by using a familiar graphics API accessed via the Shape class.


Roadmap
===========================

Improve performance of triangulator by using trapezoidalisation to pre-process polygons fed to the ear-clipping algorithm.

Provide an extensive, and easily extendable library of low-level primitives (Planes, NGons, Arcs etc). These will be many times more performant to use than drawing them manually via mutliple moveTo()/lineTo() calls (which end up being processed by the triangulator)

Provide an extended library of off-the-shelf vertex/fragment shaders for commonly desired effects (reccomendations/votes welcome).

Add support for 'holes' on fills.



Starling Framework: the GPU powered 2D Flash API
================================================

What is Starling?
-----------------

Starling is an ActionScript 3 library that mimics the conventional Flash display tree architecture. In contrast to conventional display objects, however, Starling "lives" entirely inside the Stage3D environment. That means that all objects are rendered directly by the GPU, which leads to a significant performance boost. 

Starling's API is not a direct 1:1 port of the Flash API. The classes were streamlined and optimized for working well with the GPU; common tasks in game development were simplified. Starling hides the Stage3D internals from developers, but makes it easy to access them for those who need to create custom display objects.

Just like its iOS sibling, the [Sparrow Framework][1], Starling aims to be as lightweight and easy to use as possible. As an Open Source project, much care was taken to make the source code easy to read, understand and extend.

Where do I find more information about Starling?
------------------------------------------------

Here are a few starting points:

* [Official Homepage](http://www.starling-framework.org)
* [API Reference](http://doc.starling-framework.org)
* [Support Forum](http://forum.starling-framework.org)
* [Starling Wiki](http://wiki.starling-framework.org)
  * [Showcase](http://wiki.starling-framework.org/games/start)
  * [Books, Courses, Tutorials](http://wiki.starling-framework.org/tutorials/start)
  * [Extensions](http://wiki.starling-framework.org/extensions/start)

[1]: http://www.sparrow-framework.org