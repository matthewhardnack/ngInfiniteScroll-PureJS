![logo](http://binarymuse.github.com/ngInfiniteScroll/images/logo-resized.png)

[![Build Status](https://travis-ci.org/BinaryMuse/ngInfiniteScroll.png?branch=master)](https://travis-ci.org/BinaryMuse/ngInfiniteScroll)

ngInfiniteScroll is a directive (refactored in PureJS) for [AngularJS](http://angularjs.org/) to evaluate an expression when the bottom of the directive's element approaches the bottom of the browser window, which can be used to implement infinite scrolling.

Demos
-----

Check out the running demos [at the ngInfiniteScroll web site](http://binarymuse.github.com/ngInfiniteScroll/demos.html).

Version Numbers
---------------

ngInfinite Scroll follows [semantic versioning](http://semver.org/) and uses the following versioning scheme:

 * Versions starting with 0 (e.g. 0.1.0, 0.2.0, etc.) are for initial development, and the API is not stable
 * Versions with an even minor version (1.0.0, 1.4.0, 2.2.0, etc.) are stable releases
 * Versions with an odd minor version (1.1.0, 1.3.0, 2.1.0, etc.) are development releases

The [download page](http://binarymuse.github.com/ngInfiniteScroll/#download) allows you to pick among various versions and specify which releases are stable (not including pre-release builds).

Getting Started
---------------

 * Download ngInfiniteScroll annd install manually or install it with [Bower](http://bower.io/) via `bower install ngInfiniteScroll-PureJS`

        <script type='text/javascript' src='path/to/angular.min.js'></script>
        <script type='text/javascript' src='path/to/ng-infinite-scroll.min.js'></script>

 * Ensure that your application module specifies `infinite-scroll` as a dependency:

        angular.module('myApplication', ['infinite-scroll']);

 * Use the directive by specifying an `infinite-scroll` attribute on an element.

        <div infinite-scroll="myPagingFunction()" infinite-scroll-distance="3"></div>

Note that neither the module nor the directive use the `ng` prefix, as that prefix is reserved for the core Angular module.

Detailed Documentation
----------------------

ngInfiniteScroll accepts several attributes to customize the behavior of the directive; detailed instructions can be found [on the ngInfiniteScroll web site](http://binarymuse.github.com/ngInfiniteScroll/documentation.html).

License
-------

ngInfiniteScroll is licensed under the MIT license. See the LICENSE file for more details.

Testing
-------

ngInfiniteScroll uses Testacular for its unit tests. Note that you will need [PhantomJS](http://phantomjs.org/) on your path, and the `grunt-cli` npm package installed globally if you wish to use grunt (`npm install -g grunt-cli`). Then, install the dependencies with `npm install`.

 * `grunt test` - continually watch for changes and run tests in PhantomJS and Chrome
 * `npm test` - run tests once in PhantomJS only
