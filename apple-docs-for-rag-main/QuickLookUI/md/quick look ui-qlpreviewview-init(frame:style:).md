

- Quick Look UI
- QLPreviewView
-  init(frame:style:) 

Initializer

# init(frame:style:)

Creates a preview view with the provided frame and style.

macOS 10.7+

``` source
@MainActor
init!(
    frame: NSRect,
    style: QLPreviewViewStyle
)
```

## Parameters 

`frame`  

The frame rectangle for the initialized `QLPreviewView` object.

`style`  

The desired style for the `QLPreviewView` object. For a list of possible styles, see QLPreviewViewStyle.

## Return Value

Returns a `QLPreviewView` object with the designated frame and style.

## Discussion

This is the designated initializer for the `QLPreviewView` class.

## See Also

### Creating a Preview View

init!(frame: NSRect)

Creates a preview view with the provided frame.

enum QLPreviewViewStyle

Styles for a Preview View.

