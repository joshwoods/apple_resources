

- UIKit
- UIDocumentBrowserViewController
-  transitionController(forDocumentAt:) 

Instance Method

# transitionController(forDocumentAt:)

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func transitionController(forDocumentAt documentURL: URL) -> UIDocumentBrowserTransitionController
```

## Parameters 

`documentURL`  

The URL of a document. Only use URLs provided by the document browser (for example, URLs passed to the delegate’s documentBrowser(_:didRequestDocumentCreationWithHandler:)method’s completion block).

## Return Value

Returns a newly instantiated transition controller. Its loadingProgress and targetView properties are both set to `nil`.

## Discussion

For the animations to function properly, you must maintain a strong reference to the transition controller until all the animation sequences are complete.

For more about using the transition controller, see UIDocumentBrowserTransitionController.

Note

In Mac apps built with Mac Catalyst, the transition controller doesn’t generate animations. macOS doesn’t use animations when opening or closing documents.

## See Also

### Animating transitions

class UIDocumentBrowserTransitionController

An object that implements the standard loading and transition animations for a document browser.

