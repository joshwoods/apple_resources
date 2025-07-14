

- UIKit
- UIDocumentBrowserAction
- UIDocumentBrowserAction.Availability
-  navigationBar 

Type Property

# navigationBar

An action that appears in the navigation bar when the user puts the document browser in Select mode.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var navigationBar: UIDocumentBrowserAction.Availability { get }
```

## Discussion

The system enables this action as soon as the user makes a valid selection, as determined by the supportedContentTypes and supportsMultipleItems properties.

Note

In Mac apps built with Mac Catalyst, the system shows navigationBar actions as menu actions.

## See Also

### Constants

static var menu: UIDocumentBrowserAction.Availability

An action that appears in the Edit Menu when the user long presses a supported document.

