# Tabs

This component is a simple navigation tab. It includes 5 tabs to navigate through by clicking the tabs.

## Sketch
![][sketch]

Doesn't really look like the sketch though.

## Sources
Examples:
- https://codepen.io/Gelsot/pen/eMOvOP
- https://codepen.io/fusco/pen/Wvzjrm
- https://codepen.io/oknoblich/pen/tfjFl

Reads:
- https://usabilitygeek.com/14-guidelines-for-web-site-tabs-usability/
- https://www.smashingmagazine.com/2009/06/module-tabs-in-web-design-best-practices-and-solutions/

## Testing
Tested IE using virtualbox windows 7 and in the devicelab.

**Working**
- IE11
![][ie11]

![][kindle]

![][nokia]

![][op]

![][lg]

![][samsung]

**Not Working**
- IE8
![][ie8-no]

A script didn't work here so I had to fix it.

![][ie8]

IE8 does not support `document.getElementsByClassName` so no toggle here.

## Core functionality

The component, without JS, is simply a list with content. If there is JS the list will be shown. If JS is enabled tabbing will be possible.

The component makes use of `getElementsByClassName` and `addEventListener`.

To use it safely we try to detect it with the following wrappers:

```
if (document.getElementsByClassName) {
	...
}
```

and 

```
if (document.addEventListener) {
	tabs[i].addEventListener('click', function() { ... });
} else {
	tabs[i].attachEvent('onclick', function() { ... });
}
```

[sketch]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/sketch.jpg

[ie11]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/ie11.png
[ie8]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/ie8.png
[ie8-no]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/ie8-no.png
[kindle]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/kindle.jpg
[nokia]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/nokia.jpg  
[op]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/op.jpg
[lg]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/lg.jpg
[samsung]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/tabs/doc/samsung.jpg