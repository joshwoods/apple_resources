

- WebKit
- DOMElement
-  image() 

Instance Method

# image()

Returns an image associated with the receiver.

macOS 10.5+

``` source
func image() -> NSImage!
```

## Discussion

Returns an `NSImage` for the receiver if it is a `DOMHTMLImageElement` object—a `DOMHTMLObjectElement` object with an image loaded or a `DOMHTMLInputElement` object of type image. Returns `nil` if there is an error loading the image or the element does not contain an image.

