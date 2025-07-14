

- File Provider
-  NSFileProviderItemDecorationIdentifier 

Structure

# NSFileProviderItemDecorationIdentifier

A decoration identifier defined in the File Provider extension’s information property list.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderItemDecorationIdentifier
```

## Topics

### Creating Decoration Identifiers

init(String)

Returns a new decoration identifier matching the provided String.

init(rawValue: String)

Returns a new decoration identifier matching the provided value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Items and metadata

struct NSFileProviderItemFields

Fields that specify which of the item’s properties have changed.

class NSFileProviderItemVersion

The version of the item’s content and its metadata.

class NSFileProviderRequest

An object that provides information about the application requesting data from the File Provider extension.

protocol NSFileProviderItemDecorating

Support for decorating items.

