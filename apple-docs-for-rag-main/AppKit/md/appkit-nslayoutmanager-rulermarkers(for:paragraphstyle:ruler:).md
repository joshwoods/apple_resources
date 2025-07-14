

- AppKit
- NSLayoutManager
-  rulerMarkers(for:paragraphStyle:ruler:) 

Instance Method

# rulerMarkers(for:paragraphStyle:ruler:)

Returns an array of text ruler objects for the current selection.

macOS

``` source
func rulerMarkers(
    for view: NSTextView,
    paragraphStyle style: NSParagraphStyle,
    ruler: NSRulerView
) -> [NSRulerMarker]
```

## Parameters 

`view`  

The text view using the layout manager.

`style`  

Sets the state of the controls in the accessory view; must not be `nil`.

`ruler`  

The ruler view whose ruler markers are returned.

## Return Value

An array of NSRulerMarker objects representing such things as left and right margins, first-line indent, and tab stops.

## Discussion

If you have turned off automatic ruler updating through the use of usesRuler so that you can do more complex things, but you still want to display the appropriate accessory view, you can use this method.

This method is invoked automatically by the `NSTextView` object using the layout manager. You should rarely need to invoke it, but you can override it to add new kinds of markers or otherwise customize ruler support.

You can set the returned ruler markers with the `NSRulerView` method markers.

## See Also

### Handling Rulers

func rulerAccessoryView(for: NSTextView, paragraphStyle: NSParagraphStyle, ruler: NSRulerView, enabled: Bool) -> NSView?

Returns the accessory view that the text system uses for its ruler.

