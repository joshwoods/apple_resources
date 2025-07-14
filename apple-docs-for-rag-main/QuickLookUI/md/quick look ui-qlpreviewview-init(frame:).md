

- Quick Look UI
- QLPreviewView
-  init(frame:) 

Initializer

# init(frame:)

Creates a preview view with the provided frame.

macOS 10.6+

``` source
@MainActor
init!(frame: NSRect)
```

## Parameters 

`frame`  

The frame rectangle for the initialized `QLPreviewView` object.

## Return Value

Returns a `QLPreviewView` object with the designated frame and the default style.

## Discussion

Calling this method is equivalent to calling init(frame:style:) with the `style` parameter being QLPreviewViewStyle.normal.

## See Also

### Creating a Preview View

init!(frame: NSRect, style: QLPreviewViewStyle)

Creates a preview view with the provided frame and style.

enum QLPreviewViewStyle

Styles for a Preview View.

