

- AccessorySetupKit
- ASPickerDisplayItem
-  ASPickerDisplayItem.SetupOptions 

Structure

# ASPickerDisplayItem.SetupOptions

Setup options offered by the accessory picker.

iOS 18.0+iPadOS 18.0+

``` source
struct SetupOptions
```

## Topics

### Creating an options instance

init(rawValue: UInt)

### Options

static var rename: ASPickerDisplayItem.SetupOptions

An option to ask the person using the app to rename the accessory.

static var confirmAuthorization: ASPickerDisplayItem.SetupOptions

An option to require the app to finish accessory authorization before showing the setup view.

static var finishInApp: ASPickerDisplayItem.SetupOptions

An option to ask the person setting up the accessory to finish additional setup in the app after the accessory is authorized.

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

### Customizing setup options

var setupOptions: ASPickerDisplayItem.SetupOptions

Custom setup options for the accessory.

var renameOptions: ASAccessory.RenameOptions

Options to allow renaming a matched accessory.

struct RenameOptions

Options that affect the behavior of an accessory renaming operation.

