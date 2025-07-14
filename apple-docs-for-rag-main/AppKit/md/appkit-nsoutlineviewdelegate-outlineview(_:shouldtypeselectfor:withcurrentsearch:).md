

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldTypeSelectFor:withCurrentSearch:) 

Instance Method

# outlineView(\_:shouldTypeSelectFor:withCurrentSearch:)

Returns a Boolean value that indicates whether type select should proceed for a given event and search string.

macOS 10.5+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldTypeSelectFor event: NSEvent,
    withCurrentSearch searchString: String?
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`event`  

The event that caused the message to be sent.

`searchString`  

The string for which searching is to proceed. The search string is `nil` if no type select has begun.

## Return Value

true if type select should proceed, otherwise false.

## Discussion

Generally, this method will be called from keyDown(with:) and the event will be a key event.

## See Also

### Supporting Type Select

func outlineView(NSOutlineView, typeSelectStringFor: NSTableColumn?, item: Any) -> String?

Returns the string that is used for type selection for a given column and item.

func outlineView(NSOutlineView, nextTypeSelectMatchFromItem: Any, toItem: Any, for: String) -> Any?

Returns the first item that matches the searchString from within the range of startItem to endItem

