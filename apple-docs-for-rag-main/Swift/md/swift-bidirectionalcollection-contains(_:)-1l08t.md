

- Swift
- BidirectionalCollection
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the collection contains the given regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func contains(_ regex: some RegexComponent) -> Bool
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

A regex to search for within this collection.

## Return Value

`true` if the regex was found in the collection, otherwise `false`.

