

- UIKit
- UIDocumentBrowserAction
-  init(identifier:localizedTitle:availability:handler:) 

Initializer

# init(identifier:localizedTitle:availability:handler:)

Instantiates and returns a new browser action item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    identifier: String,
    localizedTitle: String,
    availability: UIDocumentBrowserAction.Availability,
    handler: @escaping ([URL]) -> Void
)
```

## Parameters 

`identifier`  

A unique identifier for the activity.

`localizedTitle`  

The title that appears in the Edit Menu or navigation bar. This title should be a String returned by NSLocalizedString.

`availability`  

A value that defines where the action can appear (in the menu, navigation bar, or both).

For a list of valid values, see UIDocumentBrowserAction.Availability.

`handler`  

A block that is called when the user triggers the action. The block takes the following parameter:

urls  
An array of URLs for the documents that the user has selected. If the action’s supportsMultipleItems property is false, this array contains one URL. Otherwise, it can contain one or more URLs.

## See Also

### Creating and configuring actions

var image: UIImage?

The action’s image displayed in the navigation bar.

var supportedContentTypes: [String]

An array of uniform type identifiers that define the types of documents that the action supports.

var supportsMultipleItems: Bool

A Boolean value that determines whether the action can be triggered on more than one document at a time.

