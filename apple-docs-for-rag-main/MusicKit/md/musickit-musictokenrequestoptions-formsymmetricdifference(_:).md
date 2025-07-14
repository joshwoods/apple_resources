

- MusicKit
- MusicTokenRequestOptions
-  formSymmetricDifference(\_:) 

Instance Method

# formSymmetricDifference(\_:)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func formSymmetricDifference(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `^` (bitwise XOR) operation on the two sets’ raw values.

