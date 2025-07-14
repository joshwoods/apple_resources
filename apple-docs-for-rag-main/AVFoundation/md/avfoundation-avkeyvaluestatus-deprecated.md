

- AVFoundation
-  AVKeyValueStatus Deprecated

Enumeration

# AVKeyValueStatus

Values that indicate the loaded status of a property.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
enum AVKeyValueStatus
```

Deprecated

Use AVAsyncProperty.Status instead.

## Topics

### Status Values

case unknown

The property value’s status is unknown.

case loading

The system is loading the property value.

case loaded

The property value is ready to use.

case failed

The system is unable to load the propery value.

case cancelled

You canceled loading a property value.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

func loadValuesAsynchronously(forKeys: [String], completionHandler: (() -> Void)?)

Tells the asset to load the values of all of the specified keys that aren’t already loaded.

**Required**

Deprecated

func statusOfValue(forKey: String, error: NSErrorPointer) -> AVKeyValueStatus

Returns a status that indicates whether a property value is immediately available without blocking the calling thread.

**Required**

Deprecated

