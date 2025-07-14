

- Swift
- RangeReplaceableCollection
-  trimPrefix(\_:) 

Instance Method

# trimPrefix(\_:)

Removes the initial elements that matches the given regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func trimPrefix(_ regex: some RegexComponent)
```

Available when `Self` conforms to `BidirectionalCollection` and `SubSequence` is `Substring`.

## Parameters 

`regex`  

The regex to remove from this collection.

