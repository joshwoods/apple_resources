

- AdAttributionKit
- Postback
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the framework supports postbacks on a person’s device.

iOS 18.0+iPadOS 18.0+Mac Catalyst

``` source
static var isSupported: Bool { get }
```

## Return Value

`true` if the current device supports postbacks; otherwise, `false`.

## Discussion

Check this value to ensure the current device supports postbacks before calling methods on a `Postback`.

