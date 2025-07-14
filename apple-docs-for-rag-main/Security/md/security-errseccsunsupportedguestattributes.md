

- Security
-  errSecCSUnsupportedGuestAttributes 

Global Variable

# errSecCSUnsupportedGuestAttributes

Cannot locate guest code using this attribute set.

Mac Catalyst 13.0+macOS 10.0+

``` source
var errSecCSUnsupportedGuestAttributes: OSStatus { get }
```

## Discussion

When calling the SecHostCreateGuest function or the SecCodeCopyGuestWithAttributes(_:_:_:_:) function, you passed a key that either isn’t understood, recognized, or supported.

