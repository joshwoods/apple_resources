

- AVKit
-  AVContentSelectionViewController 

Class

# AVContentSelectionViewController

A view controller for providing additional UI to the multiview experience.

visionOS 2.0+

``` source
@MainActor @objc(AVContentSelectionViewController) @preconcurrency
class AVContentSelectionViewController
```

## Overview

Subclass or use view controller containment to add additional UI elements to the multiview experience.

## Topics

### Creating a view controller.

init?(coder: NSCoder)

Creates a view controller with data in an unarchiver.

init(nibName: String?, bundle: Bundle?)

Creates a view controller with the nib file in the specified bundle.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Providing additional UI

var contentSelectionViewController: AVContentSelectionViewController?

A view controller that presents a user interface to select additional video content to display.

