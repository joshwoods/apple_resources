

- UIKit
- NSTextRange
-  contains(\_:) 

Instance Method

# contains(\_:)

Determines if the text location you specify is in the current text range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func contains(_ location: any NSTextLocation) -> Bool
```

## Parameters 

`location`  

An NSTextLocation.

## Return Value

Returns `true` if the location is in the range otherwise `false` .

## See Also

### Finding text within the text range

func contains(NSTextRange) -> Bool

Determines if the text range you specify is in the current text range.

