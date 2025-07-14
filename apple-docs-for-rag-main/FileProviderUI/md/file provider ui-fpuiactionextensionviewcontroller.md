

- File Provider UI
-  FPUIActionExtensionViewController 

Class

# FPUIActionExtensionViewController

The custom user interface used to perform a selected action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor
class FPUIActionExtensionViewController
```

## Mentioned in 

Adding Actions to the Context Menu

## Overview

Subclass this view controller to provide the user interface for your actions.

No matter how many actions you define, your File Provider UI extension has only one `FPUIActionExtensionViewController` subclass. When the user selects one of your actions, the system instantiates a copy of your subclass, calls its prepare(forAction:itemIdentifiers:) method, and presents it to the user.

Your subclass must do the following:

- Override the prepare(forAction:itemIdentifiers:) method to check the action identifiers and present an appropriate user interface for the selected actions.

- Provide some sort of feedback, even if the action doesn’t require interaction with the user. For example, present a view that quickly fades out and automatically completes the action.

- Call the extensionContext object’s cancelRequest(withError:) or completeRequest() method when the action is finished to complete the action.

## Topics

### Working with Actions

func prepare(forAction: String, itemIdentifiers: [NSFileProviderItemIdentifier])

Performs any necessary setup or configuration for the specified action.

func prepare(forError: any Error)

Performs any necessary setup or configuration when an authentication error occurs.

var extensionContext: FPUIActionExtensionContext

The extension context provided by the host app.

class FPUIActionExtensionContext

An extension context provided to File Provider UI extensions.

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

### Document Browser Customization

Adding Actions to the Context Menu

Present custom actions from your File Provider extension in the system’s file browser.

