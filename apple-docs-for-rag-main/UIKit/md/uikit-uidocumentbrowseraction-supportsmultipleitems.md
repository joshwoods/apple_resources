

- UIKit
- UIDocumentBrowserAction
-  supportsMultipleItems 

Instance Property

# supportsMultipleItems

A Boolean value that determines whether the action can be triggered on more than one document at a time.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var supportsMultipleItems: Bool { get set }
```

## Discussion

This property defaults to true.

## See Also

### Creating and configuring actions

init(identifier: String, localizedTitle: String, availability: UIDocumentBrowserAction.Availability, handler: ([URL]) -> Void)

Instantiates and returns a new browser action item.

var image: UIImage?

The action’s image displayed in the navigation bar.

var supportedContentTypes: [String]

An array of uniform type identifiers that define the types of documents that the action supports.

