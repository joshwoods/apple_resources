

- Core Text
-  CTTextTabGetLocation(\_:) 

Function

# CTTextTabGetLocation(\_:)

Returns the tab’s ruler location.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTTextTabGetLocation(_ tab: CTTextTab) -> Double
```

## Parameters 

`tab`  

The tab whose location is obtained.

## Return Value

The tab’s ruler location relative to the back margin.

## See Also

### Getting Text Tab Data

func CTTextTabGetAlignment(CTTextTab) -> CTTextAlignment

Returns the text alignment of the tab.

func CTTextTabGetOptions(CTTextTab) -> CFDictionary?

Returns the dictionary of attributes associated with the tab.

