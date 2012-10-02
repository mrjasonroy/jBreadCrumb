## Update - jBreadCrumb 1.1

With a little help from jquery user "mikejbond", the chevron overlay div no
longer needs to be part of the HTML, it is inserted dynamically. You may still
want include it if you want to cache image on page load. Also, the easing
plugin is no longer required, the animation will default to "swing" easing. I
still recommend "easeOutQuad" for the best looking animation, but it's not
necessary.

## Explanation

This collapsible breadcrumb was developed to deal with deeply nested,
verbosely named pages. Rather than limit the amount of elements shown on the
sever side, we decided to go with a client side solution for usability and SEO
reasons. It also turned out nice to look at and fun to play with.

It is smart in the sense that it collapses based upon the amount and length of
the elements in the set. The breadcrumb uses a semitransparent .png overlay to
achieve the gradient effect seen on the elements. Visually, it helps to show a
"peek" at what is underneath.

Oh, and it's compatible with ie 6, ie 7 and all standards compliant browsers.

To use the plugin, it's as simple as the code below.

    
    jQuery(document).ready(function()
    {
    	jQuery("#breadCrumb").jBreadCrumb();
    })

The only additional jQuery plugin required is the [easing
plugin](http://gsgd.co.uk/sandbox/jquery/easing/) written by GSGD. The plugin
uses Robert Penner's wonderful easing equations that anyone from a flash
background is familiar with, I love 'easeOutQuad', it makes things so
smooooth.

If you don't want to use the plugin, set the options to use the normal "swing"
(esentially "easeInOut") or "linear" easing provided by jQuery. The easing
equations will no longer be necessary.

    
    jQuery(document).ready(function()
    {
    	jQuery("#breadCrumb").jBreadCrumb({easing:'swing'});
    })
    

Or, set it globally

    
    
    jQuery.fn.jBreadCrumb.defaults.easing = 'linear';
    

There are a lot of options in there, you can adjust many of the features
pretty easily through the options. Have fun with it.

Written by Jason Roy for CompareNetworks Inc.

Copyright (c) 2008 CompareNetworks Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

### Get jQuery.jBreadCrumb 1.1

You can download the files necessary to use the plugin above
