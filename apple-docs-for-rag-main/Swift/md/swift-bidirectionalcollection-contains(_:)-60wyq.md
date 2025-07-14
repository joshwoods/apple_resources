

- Swift
- BidirectionalCollection
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether this collection contains a match for the regex, where the regex is created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func contains(@RegexComponentBuilder _ content: () -> some RegexComponent) -> Bool
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns a regex to search for within this collection.

## Return Value

`true` if the regex returned by `content` matched anywhere in this collection, otherwise `false`.

