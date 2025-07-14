

- Group Activities
- BroadcastOptions
-  formIntersection(\_:) 

Instance Method

# formIntersection(\_:)

Removes all elements of this option set that are not also present in the given set.

Group ActivitiesSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
mutating func formIntersection(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `&` (bitwise AND) operation on the two sets’ raw values.

