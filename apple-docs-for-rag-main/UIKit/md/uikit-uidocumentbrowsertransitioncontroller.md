

- UIKit
-  UIDocumentBrowserTransitionController 

Class

# UIDocumentBrowserTransitionController

An object that implements the standard loading and transition animations for a document browser.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDocumentBrowserTransitionController
```

## Overview

Each transition controller is associated with a document in the document browser. The transition controller can provide two separate animation sequences for this document:

- If you set the loadingProgress property, the document browser shows the loading progress in the document’s thumbnail.

- If you set the targetView property, the transition controller acts as a UIViewControllerAnimatedTransitioning object, providing a custom transition between the document’s thumbnail and the target view. This transitioning object can be used both when presenting and when dismissing the document.

You don’t instantiate instances of UIDocumentBrowserTransitionController yourself. Instead, call the document browser’s transitionController(forDocumentURL:) method to get a transition controller for the specified document.

Note

In Mac apps built with Mac Catalyst, the transition controller doesn’t trigger animations because the macOS design doesn’t use animations for opening or closing documents.

## Topics

### Animating transitions

var loadingProgress: Progress?

A progress object that tracks a document as it loads.

var targetView: UIView?

The target view for transition animations when presenting or dismissing the transition controller’s document.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIViewControllerAnimatedTransitioning

## See Also

### Related Documentation

class UIDocumentBrowserViewController

A view controller for browsing and performing actions on documents that you store locally and in the cloud.

### Animating transitions

func transitionController(forDocumentAt: URL) -> UIDocumentBrowserTransitionController

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

