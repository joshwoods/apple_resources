

- AppKit
- NSBrowserDelegate
-  browserColumnConfigurationDidChange(\_:) 

Instance Method

# browserColumnConfigurationDidChange(\_:)

Used by clients to implement their own column width persistence.

macOS 10.10+

``` source
@MainActor
optional func browserColumnConfigurationDidChange(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named columnConfigurationDidChangeNotification.

## Discussion

This method applies only to browsers with resize type NSBrowser.ColumnResizingType.userColumnResizing. It is invoked when the setWidth(_:ofColumn:) method of NSBrowser is used to change the width of any browser columns or when the user resizes any columns. If the user resizes more than one column, a single notification is posted when the user is finished resizing.

## See Also

### Related Documentation

func setWidth(CGFloat, ofColumn: Int)

Sets the width of the specified column.

### Sizing

func browser(NSBrowser, shouldSizeColumn: Int, forUserResize: Bool, toWidth: CGFloat) -> CGFloat

Used to determine a column’s initial size.

func browser(NSBrowser, sizeToFitWidthOfColumn: Int) -> CGFloat

Returns the ideal width for a column.

func browser(NSBrowser, heightOfRow: Int, inColumn: Int) -> CGFloat

Specifies the height of the specified row in the specified column.

