

- Core HID
- HIDUsage
-  init(page:usage:) 

Initializer

# init(page:usage:)

Creates a HID usage page from raw page and usage values.

macOS 15.0+

``` source
init(
    page: UInt16,
    usage: UInt16?
)
```

## Discussion

Unsupported cases are returned as HIDUsage.generic(_:_:).

