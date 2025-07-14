

- PassKit (Apple Pay and Wallet)
-  PKAddSecureElementPassViewController 

Class

# PKAddSecureElementPassViewController

A view controller that manages the addition of secure element payment passes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
class PKAddSecureElementPassViewController
```

## Topics

### Creating a view controller

init?(configuration: PKAddSecureElementPassConfiguration, delegate: (any PKAddSecureElementPassViewControllerDelegate)?)

Creates a view controller using the specified pass configuration.

### Responding to the life cycle of a pass

var delegate: (any PKAddSecureElementPassViewControllerDelegate)?

An object that acts as the view controller’s delegate.

protocol PKAddSecureElementPassViewControllerDelegate

The methods for responding to the life cycle events of a Secure Element pass.

### Validating pass configuration

class func canAddSecureElementPass(configuration: PKAddSecureElementPassConfiguration) -> Bool

Returns a Boolean value that indicates whether PassKit can create a Secure Element pass using the specified configuration.

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

class PKPass

An object that represents a single pass.

class PKAddPassesViewController

Lets your app show a pass and prompt the user to add that pass to the pass library.

struct AsyncShareablePassConfiguration

class PKShareSecureElementPassViewController

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

