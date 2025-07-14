

- PassKit (Apple Pay and Wallet)
-  AsyncShareablePassConfiguration 

Structure

# AsyncShareablePassConfiguration

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
struct AsyncShareablePassConfiguration where Content : View
```

## Topics

### Creating the configuration

init(metadata: [PKShareablePassMetadata], action: PKAddShareablePassConfigurationPrimaryAction, content: (AsyncShareablePassConfiguration&lt;Content>.Result) -> Content)

enum Result

## Relationships

### Conforms To

- Sendable
- View

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

class PKShareSecureElementPassViewController

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

