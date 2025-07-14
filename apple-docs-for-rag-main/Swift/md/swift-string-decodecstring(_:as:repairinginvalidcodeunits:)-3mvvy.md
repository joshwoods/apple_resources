

- Swift
- String
-  decodeCString(\_:as:repairingInvalidCodeUnits:) 

Type Method

# decodeCString(\_:as:repairingInvalidCodeUnits:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func decodeCString(
    _ cString: [Encoding.CodeUnit],
    as encoding: Encoding.Type,
    repairingInvalidCodeUnits isRepairing: Bool = true
) -> (result: String, repairsMade: Bool)? where Encoding : _UnicodeEncoding
```

