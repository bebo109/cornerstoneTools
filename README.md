[![NPM version][npm-version-image]][npm-url] [![NPM downloads][npm-downloads-image]][npm-url] [![MIT License][license-image]][license-url] [![Build Status][travis-image]][travis-url]
[![Coverage Status][coverage-image]][coverage-url]

cornerstoneTools
================

`cornerstoneTools` is a library built on top of [cornerstone](https://github.com/chafey/cornerstone) that provides
a set of common tools needed in medical imaging to work with images and stacks of images.

* View [live examples](https://rawgithub.com/chafey/cornerstoneTools/master/examples/index.html) of individual tools
* Take a peak at a [simple image viewer](http://chafey.github.io/cornerstoneDemo/) built on cornerstone
* Check out a [more fully featured solution](http://viewer.ohif.org/) maintained by [OHIF](http://ohif.org/)


Features
--------

<!-- 5 columns looks great on desktop, but 4 column table supports mobile better -->
<table>
  <!-- Image Row -->
  <tr>
    <td>
      ![WW/WC Tool Example](https://github.com/dannyrb/cornerstoneTools/raw/b5f1595d5ecbb021efcdb6640efc5d49751e3a08/examples/00-tool-images/wwwc.gif)
    </td>
    <td>
      ![Zoom Tool Example](https://github.com/dannyrb/cornerstoneTools/raw/e0a85b1dfad09cae76f47dc7629e3eb03c70135c/examples/00-tool-images/zoom.gif)
    </td>
    <td>
      ![Pan Tool Example](https://github.com/dannyrb/cornerstoneTools/raw/e0a85b1dfad09cae76f47dc7629e3eb03c70135c/examples/00-tool-images/pan.gif)
    </td>
    <td>
      ![Length Tool Example](https://github.com/dannyrb/cornerstoneTools/raw/e0a85b1dfad09cae76f47dc7629e3eb03c70135c/examples/00-tool-images/length.gif)
    </td>
  <tr>
  <!-- Name Row -->
  <tr>
    <td>WW/WC</td>
    <td>Zoom</td>
    <td>Pan</td>
    <td>Length</td>
  </tr>
  <!-- External Links Row -->
  <tr>
    <td>
      [Example](https://rawgit.com/chafey/cornerstoneTools/master/examples/allImageTools/index.html) / [Source](https://github.com/dannyrb/cornerstoneTools/blob/074c012323786744e45415f82a21582f65689923/src/imageTools/wwwc.js)
    </td>
    <td>
      [Example](https://rawgit.com/chafey/cornerstoneTools/master/examples/allImageTools/index.html)	/ [Source](https://github.com/chafey/cornerstoneTools/blob/master/src/imageTools/zoom.js)
    </td>
    <td>
      [Example](https://rawgit.com/chafey/cornerstoneTools/master/examples/allImageTools/index.html)	/ [Source](https://github.com/chafey/cornerstoneTools/blob/master/src/imageTools/pan.js)
    </td>
    <td>
      [Example](https://rawgit.com/chafey/cornerstoneTools/master/examples/allImageTools/index.html)	/ [Source](https://github.com/chafey/cornerstoneTools/blob/master/src/imageTools/length.js)
    </td>
  </tr>
  <!-- Buffer Row -->
  <tr>
    <td colspan="4">&nbsp;</td>
  </tr>
   <!-- Image Row -->
  <tr>
    <td>
      ![Rectangle ROI Tool Example](https://github.com/dannyrb/cornerstoneTools/raw/e0a85b1dfad09cae76f47dc7629e3eb03c70135c/examples/00-tool-images/rectangle-roi.gif)
    </td>
    <td>
      ![Elliptical ROI Tool Example](https://placehold.it/150)
    </td>
    <td>
      ![Pixel Probe Tool Example](https://placehold.it/150)
    </td>
    <td>
      ![Angle Tool Example](https://placehold.it/150)
    </td>
  <tr>
  <!-- Name Row -->
  <tr>
    <td>Rectangle ROI</td>
    <td>Elliptical ROI</td>
    <td>Pixel Probe</td>
    <td>Angle</td>
  </tr>
  <!-- External Links Row -->
  <tr>
    <td>
      [Example](https://rawgit.com/chafey/cornerstoneTools/master/examples/allImageTools/index.html)	/ [Source](https://github.com/chafey/cornerstoneTools/blob/master/src/imageTools/rectangleRoi.js)
    </td>
    <td>
      [Example]()	/ [Source]()
    </td>
    <td>
      [Example]()	/ [Source]()
    </td>
    <td>
      [Example]()	/ [Source]()
    </td>
  </tr>
  <!-- Buffer Row -->
  <tr>
    <td colspan="4">&nbsp;</td>
  </tr>
  <!-- Image Row -->
  <tr>
    <td>
      ![Scroll Tool Example](https://placehold.it/150)
    </td>
    <td>
      ![Cine / Playing Clips Tool Example](https://placehold.it/150)
    </td>
    <td>
      ![Cross reference lines Tool Example](https://placehold.it/150)
    </td>
    <td>
      ![Placeholder Example](https://placehold.it/150)
    </td>
  <tr>
  <!-- Name Row -->
  <tr>
    <td>Scroll</td>
    <td>Cine / Playing Clips</td>
    <td>Reference Lines</td>
    <td>TBD</td>
  </tr>
  <!-- External Links Row -->
  <tr>
    <td>
      [Example]()	/ [Source]()
    </td>
    <td>
      [Example]()	/ [Source]()
    </td>
    <td>
      [Example]()	/ [Source]()
    </td>
    <td>
      [Example]()	/ [Source]()
    </td>
  </tr>
</table>


**Other Features:**

* Time Series Tools
  * Play
  * Scroll
  * Probe
* Synchronization Tools
  * By image index
  * By image position
  * By zoom and pan
  * By ww/wc and inversion
* Measurement Manager
* Support for binding each tool to different mouse inputs:
  * Left mouse button
  * Middle mouse button
  * Right mouse button
  * Mouse Wheel
* Support for touch based gestures
  * Drag
  * Pinch
* Tool framework that can be used to simplify development of new tools that work in a consistent manner with the included
  tools
* Provides API to access measurement data for serialization purposes (e.g. save measurements to database)


Getting Started
---------------

### Install

**Via NPM:** (preferred)

`npm install --save cornerstone-tools`


**Get a packaged source file:**

[UNPKG](https://unpkg.com/#/) offers a quick/neat solution for grabbing versioned copies of the source. For example:

`https://unpkg.com/<package-name>@<package-version>/path/to/desired-file.js`

* For development, to get the latest minified source:
    * `<script src="https://unpkg.com/cornerstone-tools"></script>`
* For production, specify a package version:
    * `<script src="https://unpkg.com/cornerstone-tools@0.9.0"></script>`


### Usage

See the [live examples](https://rawgithub.com/chafey/cornerstoneTools/master/examples/index.html) and [wiki](https://github.com/chafey/cornerstoneTools/wiki) for documentation on how to use this library


**A common setup when using modules:**

````javascript
// Load NPM packages
import $ from 'jquery';                           // npm install --save jquery
import Hammer from 'hammerjs';                    // npm install --save hammerjs
import * as cornerstone from 'cornerstone-core';  // npm install --save cornerstone-core
import * as cornerstoneTools from 'cornerstone-tools';

// Specify external dependencies
cornerstone.external.$ = $;
cornerstoneTools.external.cornerstone = cornerstone;
cornerstoneTools.external.$ = $;
cornerstoneTools.external.Hammer = Hammer;
````

*Note: `cornerstoneTools.external`'s only need to be specified in `cornerstone-tools` versions 1.0.0+


**A common setup when using package source files:**

````javascript
// Load Packaged Sources
<script src="https://unpkg.com/jquery@3.2.1/dist/jquery.js"></script>
<script src="https://unpkg.com/hammerjs@2.0.8/hammer.js"></script>
<script src="https://unpkg.com/cornerstone-core@1.1.0/dist/cornerstone.min.js"></script>
<script src="https://unpkg.com/cornerstone-tools@1.0.2/dist/cornerstoneTools.min.js"></script>

// Specify external dependencies
cornerstoneTools.external.cornerstone = cornerstone;
cornerstoneTools.external.$ = $;
cornerstoneTools.external.Hammer = Hammer;
````

*Note: `cornerstoneTools.external`'s only need to be specified in `cornerstone-tools` versions 1.0.0+


Contributing
------------

We love contributions, and we have plenty of work queued up for all skill levels. If you have an idea, feel free to create a new topic on [our community discussion board](https://groups.google.com/forum/#!forum/cornerstone-platform), or comment on an existing [enhancement](https://github.com/chafey/cornerstoneTools/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement), [up-for-grabs](https://github.com/chafey/cornerstoneTools/issues?q=is%3Aissue+is%3Aopen+label%3A%22up+for+grabs%22), [bug](https://github.com/chafey/cornerstoneTools/issues?q=is%3Aissue+is%3Aopen+label%3Abug), [documentation](https://github.com/chafey/cornerstoneTools/labels/documentation) issue. A quick "here is how I intend to approach this problem", with sign-off from someone like @swederik, will go a long way toward increasing the chances your hard work will be merged :+1:

**How To Contribute:**

1. Fork this repository
2. Clone the forked repository
3. Before committing code, create a branch-per-feature, or branch-per-bug
4. Create pull requests against `chafey/cornerstoneTools/master`

**What To Contribute:**

If you're looking to get your feet wet, start by:

- Read existing [wiki documentation](https://github.com/chafey/cornerstoneTools/wiki) as you implement your solution. Notice any holes? Fill them in.
- Can't find an [example of a tool](https://rawgit.com/chafey/cornerstoneTools/master/examples/index.html)? Or think an example can be improved? Improve it.
- Creating your first tool and learned some lessons along the way? Add documentation to help others.

Can't think of anything? Weigh in on and claim an [outstanding issue in the backlog](https://github.com/chafey/cornerstoneTools/issues).


Versioning
----------

cornerstoneTools will be maintained under the [Semantic Versioning Guidelines](http://semver.org) as much as possible. Releases will be numbered with the following format:

`<major>.<minor>.<patch>`

And constructed with the following guidelines:

* Breaking backward compatibility bumps the major (and resets the minor and patch)
  - Information on how to navigate breaking changes will be included in our [Change Log](https://github.com/chafey/cornerstoneTools/blob/master/changelog.md)
* New additions, including new icons, without breaking backward compatibility bumps the minor (and resets the patch)
* Bug fixes, changes to brand logos, and misc changes bumps the patch


Build System
------------

This project uses webpack to build the software.

**Requirements:**

* [NodeJs](http://nodejs.org).

**Common Tasks:**


Update dependencies (after each pull):
> npm install

Running the build:
> npm start

Automatically running the build and unit tests after each source change:
> npm run watch

Backlog
------------

* Updating related handles while resizing (e.g. resize top left handle of a rect and update the bottom left and top right as it changes)
* measurement calibration tool
* Config object that allows tool appearance to be customized (e.g. line color, text color, handle size, shape, etc)
* automatically disabling tools when the enabled element is disabled
* reconsider the state management api, it is a bit clunky
* add support for pointer events as an input source
* Reference line renderer for first/last/active
* Annotations (e.g. text, arrows, circles)
* Move all API documentation from [wiki](https://github.com/chafey/cornerstoneTools/wiki) into markdown in a doc folder
* key press input source - so user can interact with tools via keyboard (e.g. scroll stack image using arrow keys)

Copyright
============
Copyright 2015 Chris Hafey [chafey@gmail.com](mailto:chafey@gmail.com)

[license-image]: http://img.shields.io/badge/license-MIT-blue.svg?style=flat
[license-url]: LICENSE

[npm-url]: https://npmjs.org/package/cornerstone-tools
[npm-version-image]: http://img.shields.io/npm/v/cornerstone-tools.svg?style=flat
[npm-downloads-image]: http://img.shields.io/npm/dm/cornerstone-tools.svg?style=flat

[travis-url]: http://travis-ci.org/chafey/cornerstoneTools
[travis-image]: https://travis-ci.org/chafey/cornerstoneTools.svg?branch=master

[coverage-url]: https://coveralls.io/github/chafey/cornerstoneTools?branch=master
[coverage-image]: https://coveralls.io/repos/github/chafey/cornerstoneTools/badge.svg?branch=master
