

- AccessorySetupKit
- ASAccessory
-  ASAccessory.RenameOptions 

Structure

# ASAccessory.RenameOptions

Options that affect the behavior of an accessory renaming operation.

iOS 18.0+iPadOS 18.0+

``` source
struct RenameOptions
```

## Topics

### Creating an options instance

init(rawValue: UInt)

### Options

static var ssid: ASAccessory.RenameOptions

An option to change an accessory’s SSID along with its display name.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

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

### Managing accessories

func renameAccessory(ASAccessory, options: ASAccessory.RenameOptions, completionHandler: ((any Error)?) -> Void)

Displays a view to rename an accessory.

func removeAccessory(ASAccessory, completionHandler: ((any Error)?) -> Void)

Removes an accessory.

