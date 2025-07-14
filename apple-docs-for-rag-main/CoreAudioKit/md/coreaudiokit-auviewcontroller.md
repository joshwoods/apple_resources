

- CoreAudioKit
-  AUViewController 

Class

# AUViewController

The base class to extend when creating a custom user interface for an audio unit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
class AUViewController
```

## Overview

This class doesn’t add any new methods or properties to its superclass, but it does conform to the NSExtensionRequestHandling protocol.

A host app can access the view controller by calling the requestViewController(completionHandler:) method on the corresponding AUAudioUnit object.

### Subclassing Notes

If an audio unit provides a custom view controller, the UI Audio Unit extension must implement a subclass of `AUViewController` and implement the AUAudioUnitFactory protocol inside the subclass.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

### Audio Units

class AUAudioUnitViewConfiguration

A configuration object that describes how to present the audio unit’s user interface.

class AUGenericView

A view that provides a generic user interface for a Cocoa audio unit.

class AUPannerView

A view that provides a specialized user interface for a Cocoa-based panner audio unit.

protocol AUCustomViewPersistentData

A protocol that defines the methods an Audio Unit host calls to manage view data.

