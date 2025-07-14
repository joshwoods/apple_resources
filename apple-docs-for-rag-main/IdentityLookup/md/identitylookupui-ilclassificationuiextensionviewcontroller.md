

- IdentityLookupUI
-  ILClassificationUIExtensionViewController 

Class

# ILClassificationUIExtensionViewController

The superclass for an Unwanted Communication Reporting extension’s principal view controller.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
class ILClassificationUIExtensionViewController
```

## Overview

Subclass this view controller to create a user interface that gathers additional information from the user about the reported communication.

## Topics

### Collecting Data from the User

func prepare(for: ILClassificationRequest)

Notifies the view controller just before the system presents it to the user.

func classificationResponse(for: ILClassificationRequest) -> ILClassificationResponse

Notifies the view controller when the user finishes entering data and presses the Done button.

### Managing the Request

var extensionContext: ILClassificationUIExtensionContext

The context for the current request.

class ILClassificationUIExtensionContext

An object that manages the state of the current request.

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
- NSTouchBarProvider
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

