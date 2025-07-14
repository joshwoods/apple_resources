

- AppKit
- NSPrintPanel
-  NSPrintPanel.AccessorySummaryKey 

Structure

# NSPrintPanel.AccessorySummaryKey

Constants that specify the accessory panel keys.

macOS

``` source
struct AccessorySummaryKey
```

## Discussion

These keys must be included in the dictionaries returned by the localizedSummaryItems() method.

## Topics

### Summary Keys

static let itemName: NSPrintPanel.AccessorySummaryKey

A key that specifies the name of the accessory panel setting.

static let itemDescription: NSPrintPanel.AccessorySummaryKey

A key that identfies the current value of the accessory panel setting.

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

### Responding to Being Loaded from a Nib File

func localizedSummaryItems() -> [[NSPrintPanel.AccessorySummaryKey : String]]

Returns an array of dictionaries containing the localized user setting summary strings.

**Required**

func keyPathsForValuesAffectingPreview() -> Set&lt;String>

Returns a set of strings identifying the key paths for any properties that might affect the built-in print preview.

