

- Swift
- BidirectionalCollection
-  starts(with:) 

Instance Method

# starts(with:)

Returns a Boolean value indicating whether the initial elements of this collection are a match for the regex created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func starts(@RegexComponentBuilder with content: () -> some RegexComponent) -> Bool
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns a regex to match at the beginning of this collection.

## Return Value

`true` if the initial elements of this collection match regex returned by `content`; otherwise, `false`.

