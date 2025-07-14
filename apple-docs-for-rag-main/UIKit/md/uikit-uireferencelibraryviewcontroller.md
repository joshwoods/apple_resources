

- UIKit
-  UIReferenceLibraryViewController 

Class

# UIReferenceLibraryViewController

A view controller that displays a standard interface for looking up the definition of a word or term.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIReferenceLibraryViewController
```

## Overview

A UIReferenceLibraryViewController object should not be used to display wordlists, create a standalone dictionary app, or republish the content in any form.

You create and initialize a reference library view controller using the init(term:) method. You pass the term to define as the parameter to this method and the definition is displayed. You can present this view controller modally or as part of another interface. On iPad, you can set the reference library view controller as the content view controller of a UIPopoverController object. Optionally, use the dictionaryHasDefinition(forTerm:) class method to check if a definition is available for a given term before creating an instance—for example, use this method if you want to change the user interface depending on whether a definition is available.

## Topics

### Creating a reference-library view controller

class func dictionaryHasDefinition(forTerm: String) -> Bool

Returns whether a definition is available for the given term.

init(term: String)

Initializes a newly created reference-library view controller to display the definition of the given term.

init(coder: NSCoder)

Creates a reference-library view controller from data in an unarchiver.

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

