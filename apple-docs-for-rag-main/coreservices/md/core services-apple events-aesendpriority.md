

- Core Services
- Apple Events
-  AESendPriority 

Type Alias

# AESendPriority

Specifies the processing priority for a sent Apple event.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AESendPriority = Int16
```

## Discussion

When you call the `AESend(_:_:_:_:_:_:_:)` function, you pass a value of type `AESendPriority` for the `sendPriority` parameter. Priority Constants for the AESend Function (Deprecated in macOS) lists the valid constant values for a variable or parameter of this type.

