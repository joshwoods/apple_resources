

- WebKit
- DOMHTMLDocument
-  createDocumentFragment(withMarkupString:baseURL:) 

Instance Method

# createDocumentFragment(withMarkupString:baseURL:)

Creates a document fragment containing the given HTML markup.

macOS 10.5+

``` source
func createDocumentFragment(
    withMarkupString markupString: String!,
    baseURL: URL!
) -> DOMDocumentFragment!
```

## Parameters 

`markupString`  

The HTML content to parse into a DOM tree.

`baseURL`  

The URI from which the content originated. Used for interpreting relative URLs.

## Return Value

A `DOMDocumentFragment` derived from the original markup string.

## Discussion

This is a convenience method for the `createDocumentFragment` method in `DOMDocument`. It creates a fragment that has the HTML markup parsed into child nodes of the fragment using the `baseURL` to resolve any relative paths for images or other resources.

## See Also

### Creating Document Fragments

func createDocumentFragment(withText: String!) -> DOMDocumentFragment!

Creates a document fragment containing the given text.

