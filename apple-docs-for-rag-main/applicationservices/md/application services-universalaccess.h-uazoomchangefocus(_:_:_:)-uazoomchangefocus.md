

- Application Services
- UniversalAccess.h
-  UAZoomChangeFocus(\_:\_:\_:) 

Function

# UAZoomChangeFocus(\_:\_:\_:)

Tells the Universal Access zoom feature where it should focus.

macOS 10.4+

``` source
func UAZoomChangeFocus(
    _ inRect: UnsafePointer!,
    _ inHighlightRect: UnsafePointer!,
    _ inType: UAZoomChangeFocusType
) -> OSStatus
```

## Parameters 

`inRect`  

The frame of the element in focus, in global 72-dot-per-inch (dpi) coordinates.

`inHighlightRect`  

The frame of the highlighted part of the element in focus, in global 72 dpi coordinates. If the whole element is in focus, and not just a smaller part of it, pass the `inRect` parameter and pass `NULL` for `inHighlightRect`.

`inType`  

A value of type UAZoomChangeFocusType.

## Return Value

Returns `noErr` if there were no problems, if Universal Access Zoom is zoomed all the way out, or if the feature is off; returns `paramErr` if `inRect` is `NULL` or if `inType` is out of range.

## Discussion

This function tells Universal Access the frame of the element in focus and the part of the element that should be in focus.

## See Also

### Miscellaneous

func UAZoomEnabled() -> Bool

Determines if the Universal Access zoom feature is enabled.

