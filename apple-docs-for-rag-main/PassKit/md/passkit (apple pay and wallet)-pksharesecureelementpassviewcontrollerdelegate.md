

- PassKit (Apple Pay and Wallet)
-  PKShareSecureElementPassViewControllerDelegate 

Protocol

# PKShareSecureElementPassViewControllerDelegate

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
protocol PKShareSecureElementPassViewControllerDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func shareSecureElementPassViewController(PKShareSecureElementPassViewController, didCreateShare: URL?, activationCode: String?)

func shareSecureElementPassViewController(PKShareSecureElementPassViewController, didFinishWith: PKShareSecureElementPassResult)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

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

class PKShareSecureElementPassViewController

class Preview

enum PKShareSecureElementPassResult

