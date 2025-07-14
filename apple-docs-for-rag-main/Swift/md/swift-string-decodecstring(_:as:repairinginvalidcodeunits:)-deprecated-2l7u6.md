

- Swift
- String
-  decodeCString(\_:as:repairingInvalidCodeUnits:) Deprecated

Type Method

# decodeCString(\_:as:repairingInvalidCodeUnits:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+visionOS 1.0+watchOS 2.0+tvOS 9.0+

``` source
static func decodeCString(
    _ cString: inout Encoding.CodeUnit,
    as encoding: Encoding.Type,
    repairingInvalidCodeUnits isRepairing: Bool = true
) -> (result: String, repairsMade: Bool)? where Encoding : _UnicodeEncoding
```

Deprecated

Use String(\_ scalar: Unicode.Scalar)

