

- Core Text
-  CTTextTabCreate(\_:\_:\_:) 

Function

# CTTextTabCreate(\_:\_:\_:)

Creates and initializes a new text tab object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTTextTabCreate(
    _ alignment: CTTextAlignment,
    _ location: Double,
    _ options: CFDictionary?
) -> CTTextTab
```

## Parameters 

`alignment`  

The tab’s alignment. This is used to determine the position of text inside the tab column. This parameter must be set to a valid CTTextAlignment value or this function returns `NULL`.

`location`  

The tab’s ruler location, relative to the back margin.

`options`  

Options to pass in when the tab is created. Currently, the only option available is kCTTabColumnTerminatorsAttributeName. This parameter is optional and can be set to `NULL` if not needed.

## Return Value

A reference to a CTTextTab object if the call was successful; otherwise, `NULL`.

