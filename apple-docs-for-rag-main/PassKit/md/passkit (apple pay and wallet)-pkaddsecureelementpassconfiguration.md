

- PassKit (Apple Pay and Wallet)
-  PKAddSecureElementPassConfiguration 

Class

# PKAddSecureElementPassConfiguration

An object that describes the configuration of a secure element payment pass.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+

``` source
class PKAddSecureElementPassConfiguration
```

## Overview

This class supports identity document configuration.

## Topics

### Managing the issuer identity

var issuerIdentifier: String?

An opaque value for the configuration.

var localizedDescription: String?

The configuration’s localized description.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PKAddCarKeyPassConfiguration
- PKAddIdentityDocumentConfiguration
- PKAddShareablePassConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### General purpose passes

class PKSecureElementPass

A pass with a credential that the device stores in a certified payment information chip.

class PKAddSecureElementPassViewController

A view controller that manages the addition of secure element payment passes.

class PKPass

An object that represents a single pass.

class PKAddPassesViewController

Lets your app show a pass and prompt the user to add that pass to the pass library.

struct AsyncShareablePassConfiguration

class PKShareSecureElementPassViewController

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

