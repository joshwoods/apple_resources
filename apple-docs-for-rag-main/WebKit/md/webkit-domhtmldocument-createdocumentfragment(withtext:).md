

- WebKit
- DOMHTMLDocument
-  createDocumentFragment(withText:) 

Instance Method

# createDocumentFragment(withText:)

Creates a document fragment containing the given text.

macOS 10.5+

``` source
func createDocumentFragment(withText text: String!) -> DOMDocumentFragment!
```

## Parameters 

`text`  

The text to convert.

## Return Value

A `DOMDocumentFragment` object derived from the source text.

## Discussion

This is a convenience method for the `createDocumentFragment` method in `DOMDocument`. This method creates a fragment that contains the supplied plain text.

## See Also

### Creating Document Fragments

func createDocumentFragment(withMarkupString: String!, baseURL: URL!) -> DOMDocumentFragment!

Creates a document fragment containing the given HTML markup.

