

- AppKit
- NSTextRange
-  contains(\_:) 

Instance Method

# contains(\_:)

Determines if the text location you specify is in the current text range.

macOS 12.0+

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

