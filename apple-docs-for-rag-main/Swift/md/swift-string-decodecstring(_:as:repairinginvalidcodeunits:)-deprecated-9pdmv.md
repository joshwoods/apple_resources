

- Swift
- String
-  decodeCString(\_:as:repairingInvalidCodeUnits:) Deprecated

Type Method

# decodeCString(\_:as:repairingInvalidCodeUnits:)

iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+iOS 8.0+

``` source
static func decodeCString(
    _ cString: String,
    as encoding: Encoding.Type,
    repairingInvalidCodeUnits isRepairing: Bool = true
) -> (result: String, repairsMade: Bool)? where Encoding : _UnicodeEncoding
```

Deprecated

Use a copy of the String argument

