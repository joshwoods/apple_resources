

- Core HID
- HIDUsage
-  usage 

Instance Property

# usage

The usage value.

macOS 15.0+

``` source
var usage: UInt16? { get }
```

## Discussion

The usage combines with the page to determine specific functionality. This may not be specified, in which case the `HIDUsage` refers to the overall page.

