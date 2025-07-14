

- PassKit (Apple Pay and Wallet)
-  PKLabeledValue 

Class

# PKLabeledValue

An object that can represent a detail about a payment card or other item.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 3.1+

``` source
class PKLabeledValue
```

## Overview

See cardDetails.

## Topics

### Creating a labeled value

init(label: String, value: String)

Instantiates a new labeled value object with the specified label and value strings.

### Labeled value properties

var label: String

A string that contains the label for the value.

var value: String

A string that contains the value associated with a label.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Common objects

class PKObject

An opaque type that acts as the superclass for the pass object.

class PKAddPassButton

Provides a button that enables users to add passes to Wallet.

struct AddPassToWalletButton

struct AddPassToWalletButtonFilter

struct AddPassToWalletButtonResponse

struct AddPassToWalletButtonStyle

