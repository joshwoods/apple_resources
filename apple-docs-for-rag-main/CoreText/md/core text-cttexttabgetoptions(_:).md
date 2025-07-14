

- Core Text
-  CTTextTabGetOptions(\_:) 

Function

# CTTextTabGetOptions(\_:)

Returns the dictionary of attributes associated with the tab.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTTextTabGetOptions(_ tab: CTTextTab) -> CFDictionary?
```

## Parameters 

`tab`  

The tab whose attributes are obtained.

## Return Value

The dictionary of attributes associated with the tab, or if no dictionary is present, `NULL`.

## See Also

### Getting Text Tab Data

func CTTextTabGetAlignment(CTTextTab) -> CTTextAlignment

Returns the text alignment of the tab.

func CTTextTabGetLocation(CTTextTab) -> Double

Returns the tab’s ruler location.

