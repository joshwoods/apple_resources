

- PassKit (Apple Pay and Wallet)
-  PKShareSecureElementPassViewController 

Class

# PKShareSecureElementPassViewController

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class PKShareSecureElementPassViewController
```

## Topics

### Initializers

init(secureElementPass: PKSecureElementPass, delegate: (any PKShareSecureElementPassViewControllerDelegate)?)

### Instance Properties

var delegate: (any PKShareSecureElementPassViewControllerDelegate)?

var promptToShareURL: Bool

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

class PKAddPassesViewController

Lets your app show a pass and prompt the user to add that pass to the pass library.

struct AsyncShareablePassConfiguration

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

