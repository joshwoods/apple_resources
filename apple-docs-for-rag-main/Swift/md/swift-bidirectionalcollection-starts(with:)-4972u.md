

- Swift
- BidirectionalCollection
-  starts(with:) 

Instance Method

# starts(with:)

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in the specified regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func starts(with regex: some RegexComponent) -> Bool
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

A regex to compare to this sequence.

## Return Value

`true` if the initial elements of the sequence matches the beginning of `regex`; otherwise, `false`.

