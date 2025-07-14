

- WebKit
- WKWebExtension
-  WKWebExtension.DataType 

Structure

# WKWebExtension.DataType

Constants for specifying data types for a WKWebExtension.DataRecord.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct DataType
```

## Topics

### Constants

static let local: WKWebExtension.DataType

Specifies local storage, including `browser.storage.local`.

static let session: WKWebExtension.DataType

Specifies session storage, including `browser.storage.session`.

static let synchronized: WKWebExtension.DataType

Specifies synchronized storage, including `browser.storage.sync`.

### Initializers

init(rawValue: String)

Creates a data type from a raw value you provide.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Structures

struct Error

Constants that indicate errors in the WKWebExtension domain.

struct Permission

Constants for specifying permission in a WKWebExtensionContext.

struct TabChangedProperties

Constants the web extension controller and web extension context use to indicate tab changes.

