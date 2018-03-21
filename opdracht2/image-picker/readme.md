# Image Picker

test


Two different image pickers:
- One mimicking a kind of CMS, where images are already uploaded which you can choose from.  - `index.html`
- One using the `input` tag with `type-"file"` - `image-picker2.html`



## `image-picker2.html`

Using `document.getElementsByTagName()`

> The getElementsByName method works differently in different browsers. In IE < 10, getElementsByName() method will also return elements that have an id attribute with the specified value. so you should be careful not to use the same string as both a name and an ID. source: https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByName

Cannot find a alternative to `FileReader` for support on < IE10.

source: https://html.spec.whatwg.org/multipage/dom.html#dom-document-getelementsbyname

