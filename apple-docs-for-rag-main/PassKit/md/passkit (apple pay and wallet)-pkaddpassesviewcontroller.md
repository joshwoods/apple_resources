

- PassKit (Apple Pay and Wallet)
-  PKAddPassesViewController 

Class

# PKAddPassesViewController

Lets your app show a pass and prompt the user to add that pass to the pass library.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class PKAddPassesViewController
```

## Overview

To add multiple passes without presenting this view controller multiple times, use the addPasses(_:withCompletionHandler:) method of PKPassLibrary.

## Topics

### Determining if the device supports adding passes

class func canAddPasses() -> Bool

Returns a Boolean value that indicates whether the device supports adding passes.

### Creating an add-passes view controller

init?(pass: PKPass)

Initializes and returns a newly created add-passes view controller with a single pass.

init?(passes: [PKPass])

Initializes and returns a newly created add-passes view controller with an array of passes.

init(issuerData: Data, signature: Data) throws

Initializes and returns a new add-passes view controller with the issuer data, and signature you provide.

### Adding passes

var delegate: (any PKAddPassesViewControllerDelegate)?

The view controller’s delegate.

protocol PKAddPassesViewControllerDelegate

Methods that an add-passes view controller’s delegate implements.

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

## See Also

### General purpose passes

class PKSecureElementPass

A pass with a credential that the device stores in a certified payment information chip.

class PKAddSecureElementPassConfiguration

An object that describes the configuration of a secure element payment pass.

class PKAddSecureElementPassViewController

A view controller that manages the addition of secure element payment passes.

class PKPass

An object that represents a single pass.

struct AsyncShareablePassConfiguration

class PKShareSecureElementPassViewController

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

