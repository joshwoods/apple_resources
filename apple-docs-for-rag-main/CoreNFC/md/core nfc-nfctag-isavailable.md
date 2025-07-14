

- Core NFC
- NFCTag
-  isAvailable 

Instance Property

# isAvailable

A Boolean value that indicates whether a detected tag is available.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
var isAvailable: Bool { get }
```

## Discussion

The value of this property is true when the tag is available in the current reader session. When a tag is removed from an RF field, it becomes unavailable.

