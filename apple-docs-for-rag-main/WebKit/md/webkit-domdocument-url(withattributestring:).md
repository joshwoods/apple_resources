

- WebKit
- DOMDocument
-  url(withAttributeString:) 

Instance Method

# url(withAttributeString:)

Constructs a URL given an attribute string.

macOS

``` source
func url(withAttributeString string: String!) -> URL!
```

## Parameters 

`string`  

The HTML attribute string to convert.

## Return Value

An `NSURL` object containing an absolute URL derived from the specified attribute string.

## Discussion

This method constructs a URL given the string value of an element attribute. Examples include the `href` attribute of a `DOMHTMLAnchorElement` object, or the `src` attribute of a `DOMHTMLImageElement` object. This method only applies to attributes that refer to URLs.

This method is similar to URLWithString: in the `NSURL` class, except that `URLWithAttributeString:` handles relative URLs automatically based on the current document’s location.

