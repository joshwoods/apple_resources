

- Core Text
-  CTTextTabGetAlignment(\_:) 

Function

# CTTextTabGetAlignment(\_:)

Returns the text alignment of the tab.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTTextTabGetAlignment(_ tab: CTTextTab) -> CTTextAlignment
```

## Parameters 

`tab`  

The tab whose text alignment is obtained.

## Return Value

The tab’s text alignment value.

## See Also

### Getting Text Tab Data

func CTTextTabGetLocation(CTTextTab) -> Double

Returns the tab’s ruler location.

func CTTextTabGetOptions(CTTextTab) -> CFDictionary?

Returns the dictionary of attributes associated with the tab.

