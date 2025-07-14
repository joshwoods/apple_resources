

- AppKit
- NSMenu
-  menuZone() Deprecated

Type Method

# menuZone()

Returns the zone from which `NSMenu` objects should be allocated.

macOS 10.0–10.11Deprecated

``` source
class func menuZone() -> NSZone!
```

## Return Value

The zone from which `NSMenu` objects should be allocated.

## Discussion

This is left in for compatibility and always returns NSDefaultMallocZone. It is not necessary to use this.

