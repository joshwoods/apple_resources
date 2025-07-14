

- BrowserEngineKit
- BETextReplacementOptions
-  formIntersection(\_:) 

Instance Method

# formIntersection(\_:)

Removes all elements of this option set that are not also present in the given set.

BrowserEngineKitSwiftiOS 17.4+iPadOS 17.4+tvOSvisionOS

``` source
mutating func formIntersection(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `&` (bitwise AND) operation on the two sets’ raw values.

