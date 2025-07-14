

- AppKit
- NSLayoutManager
-  rulerAccessoryView(for:paragraphStyle:ruler:enabled:) 

Instance Method

# rulerAccessoryView(for:paragraphStyle:ruler:enabled:)

Returns the accessory view that the text system uses for its ruler.

macOS

``` source
func rulerAccessoryView(
    for view: NSTextView,
    paragraphStyle style: NSParagraphStyle,
    ruler: NSRulerView,
    enabled isEnabled: Bool
) -> NSView?
```

## Parameters 

`view`  

The text view using the layout manager.

`style`  

Sets the state of the controls in the accessory view; must not be `nil`.

`ruler`  

The ruler view whose accessory view is returned.

`isEnabled`  

If true, the accessory view is enabled and accepts mouse and keyboard events; if false it’s disabled.

## Return Value

The accessory view containing tab wells, text alignment buttons, and so on.

## Discussion

If you have turned off automatic ruler updating through the use of usesRuler so that you can do more complex things, but you still want to display the appropriate accessory view, you can use this method.

This method is invoked automatically by the NSTextView object using the layout manager. You should rarely need to invoke it, but you can override it to customize ruler support. If you do use this method directly, note that it neither installs the ruler accessory view nor sets the markers for the NSRulerView object. You must install the accessory view into the ruler using the NSRulerView method accessoryView. To set the markers, use rulerMarkers(for:paragraphStyle:ruler:) to get the markers needed, and then send markers to the ruler.

## See Also

### Handling Rulers

func rulerMarkers(for: NSTextView, paragraphStyle: NSParagraphStyle, ruler: NSRulerView) -> [NSRulerMarker]

Returns an array of text ruler objects for the current selection.

