

- Swift
- BidirectionalCollection
-  trimmingPrefix(\_:) 

Instance Method

# trimmingPrefix(\_:)

Returns a new collection of the same type by removing the initial elements that matches the given regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func trimmingPrefix(_ regex: some RegexComponent) -> Self.SubSequence
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

The regex to remove from this collection.

## Return Value

A collection containing the elements that does not match `regex` from the start.

