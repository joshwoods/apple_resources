

- WebKit
- WKWebExtension
-  WKWebExtension.TabChangedProperties 

Structure

# WKWebExtension.TabChangedProperties

Constants the web extension controller and web extension context use to indicate tab changes.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct TabChangedProperties
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var URL: WKWebExtension.TabChangedProperties

Indicates the URL changed.

static var loading: WKWebExtension.TabChangedProperties

Indicates the loading state changed.

static var muted: WKWebExtension.TabChangedProperties

Indicates the muted state changed.

static var pinned: WKWebExtension.TabChangedProperties

Indicates the pinned state changed.

static var playingAudio: WKWebExtension.TabChangedProperties

Indicates the audio playback state changed.

static var readerMode: WKWebExtension.TabChangedProperties

Indicates the reader mode state changed.

static var size: WKWebExtension.TabChangedProperties

Indicates the size changed.

static var title: WKWebExtension.TabChangedProperties

Indicates the title changed.

static var zoomFactor: WKWebExtension.TabChangedProperties

Indicates the zoom factor changed.

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

### Structures

struct DataType

Constants for specifying data types for a WKWebExtension.DataRecord.

struct Error

Constants that indicate errors in the WKWebExtension domain.

struct Permission

Constants for specifying permission in a WKWebExtensionContext.

