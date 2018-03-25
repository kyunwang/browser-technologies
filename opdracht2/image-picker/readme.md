# Image Picker

There are two simple components made for this pattern.

Two different image pickers:
- One mimicking a kind of CMS, where images are already uploaded which you can choose from.  - `index.html`
- One using the `input` tag with `type-"file"` - `image-picker2.html`

## Sketch

![][sketch]

This is the sketch for the imagepicker


## `image-picker2.html`

- IE11
Using `document.getElementsByTagName()`
![][2-ie11]

- IE8
Working but the preview does not work as < IE10  does not support `FileReader`
![][2-ie8]
> The getElementsByName method works differently in different browsers. In IE < 10, getElementsByName() method will also return elements that have an id attribute with the specified value. so you should be careful not to use the same string as both a name and an ID. source: https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByName

Cannot find a alternative to `FileReader` for support on < IE10.

source:
- https://html.spec.whatwg.org/multipage/dom.html#dom-document-getelementsbyname
- https://caniuse.com/#search=filereader





## `index.html`

This component is a simulation of a situation where you already have a selection images or have already uploaded images to a CMS for instance.

It should be a form with one selectable items max, so I made it with checkboxes.

## Testing
Tested IE using virtualbox windows 7 and in the devicelab.

**Working**
- IE11
![][ie11]

<!-- ![][kindle]

![][nokia] -->

![][op]

<!-- ![][lg]

![][samsung] -->

**Not Working**
- IE8
Defining the `nextElementSibling` and adding to the `prototype` works, but because `pointer-events` is not supported we cannot click on the label.
![][ie8]


## Sources
[sketch]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/sketch.jpg



[2-ie11]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker2/ie11.png
[2-ie8]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker2/ie8.png


[ie11]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/ie11.png
[ie8]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/ie8.png
[ie8-no]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/ie8-no.png
[kindle]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/kindle.jpg
[nokia]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/nokia.jpg  
[op]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/op.jpg
[lg]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/lg.jpg
[samsung]: https://github.com/kyunwang/browser-technologies/blob/master/opdracht2/image-picker/doc/picker1/samsung.jpg