

- PassKit (Apple Pay and Wallet)
-  PKRadioTechnology 

Structure

# PKRadioTechnology

Constants that describe the type of wireless radio technology that a pass uses.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOSvisionOS 1.0+watchOS 7.3+

``` source
struct PKRadioTechnology
```

## Topics

### Reading the radio technology type

static var NFC: PKRadioTechnology

An identifier that indicates the near field communication (NFC) radio frequency communication technology.

static var bluetooth: PKRadioTechnology

An identifier that indicates the Bluetooth radio frequency communication technology.

### Creating a radio technology object

init(rawValue: UInt)

Creates a radio technology object of the specified type.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Setting the wireless radio technology

var supportedRadioTechnologies: PKRadioTechnology

The wireless radio technology that the key uses.

