

- Swift
- String
- String.UnicodeScalarView
-  reserveCapacity(\_:) 

Instance Method

# reserveCapacity(\_:)

Reserves enough space in the view’s underlying storage to store the specified number of ASCII characters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func reserveCapacity(_ n: Int)
```

## Parameters 

`n`  

The minimum number of ASCII character’s worth of storage to allocate.

## Discussion

Because a Unicode scalar value can require more than a single ASCII character’s worth of storage, additional allocation may be necessary when adding to a Unicode scalar view after a call to `reserveCapacity(_:)`.

Complexity

O(*n*), where *n* is the capacity being reserved.

