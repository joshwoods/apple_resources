

- Core HID
- HIDUsage
-  page 

Instance Property

# page

The usage page value.

macOS 15.0+

``` source
var page: UInt16 { get }
```

## Discussion

This value determines the broader category of the functionality. This must always be specified, as a usage doesn’t have meaning without a page.

