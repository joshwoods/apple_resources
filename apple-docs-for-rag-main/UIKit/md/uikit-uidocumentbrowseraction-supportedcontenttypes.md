

- UIKit
- UIDocumentBrowserAction
-  supportedContentTypes 

Instance Property

# supportedContentTypes

An array of uniform type identifiers that define the types of documents that the action supports.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var supportedContentTypes: [String] { get set }
```

## Discussion

The action can be triggered only on documents that are allowed by both the action’s supportedContentTypes property and the document browser’s allowedContentTypes property.

By default, this property contains only the `public.item` uniform type identifier (UTI)—indicating that there are no additional restrictions on document types.

To further restrict the supported documents, assign an array that contains a more restricted set of UTIs. These UTIs should define a subset of the UTIs supported by the document browser.

For more about UTIs, see Uniform Type Identifiers Reference.

## See Also

### Creating and configuring actions

init(identifier: String, localizedTitle: String, availability: UIDocumentBrowserAction.Availability, handler: ([URL]) -> Void)

Instantiates and returns a new browser action item.

var image: UIImage?

The action’s image displayed in the navigation bar.

var supportsMultipleItems: Bool

A Boolean value that determines whether the action can be triggered on more than one document at a time.

