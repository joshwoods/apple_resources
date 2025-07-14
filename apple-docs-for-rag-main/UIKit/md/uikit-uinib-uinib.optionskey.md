

- UIKit
- UINib
-  UINib.OptionsKey 

Structure

# UINib.OptionsKey

Options that specify how to unarchive and instantiate the nib.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct OptionsKey
```

## Topics

### Keys

static let externalObjects: UINib.OptionsKey

The replacements for any proxy objects in the nib file.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving objects from the nib file

func instantiate(withOwner: Any?, options: [UINib.OptionsKey : Any]?) -> [Any]

Unarchives and instantiates the in-memory contents of the nib object’s nib file, creating a distinct object tree and set of top-level objects.

