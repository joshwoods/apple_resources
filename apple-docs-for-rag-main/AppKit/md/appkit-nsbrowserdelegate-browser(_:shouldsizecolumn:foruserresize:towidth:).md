

- AppKit
- NSBrowserDelegate
-  browser(\_:shouldSizeColumn:forUserResize:toWidth:) 

Instance Method

# browser(\_:shouldSizeColumn:forUserResize:toWidth:)

Used to determine a column’s initial size.

macOS 10.0+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    shouldSizeColumn columnIndex: Int,
    forUserResize: Bool,
    toWidth suggestedWidth: CGFloat
) -> CGFloat
```

## Parameters 

`browser`  

The browser.

`columnIndex`  

The index of the column to size.

`forUserResize`  

Currently, this is always set to false.

`suggestedWidth`  

The suggested width for the column.

## Return Value

The delegate’s desired initial width for a newly added column. If you want to accept the suggested width, return `suggestedWidth`. If you return `0` or a size too small to display the resize handle and a portion of the column, the actual size used will be larger than the size you requested.

## Discussion

This method applies only to browsers with resize type NSBrowser.ColumnResizingType.noColumnResizing or NSBrowser.ColumnResizingType.userColumnResizing (see NSBrowser.ColumnResizingType).

## See Also

### Related Documentation

func setWidth(CGFloat, ofColumn: Int)

Sets the width of the specified column.

### Sizing

func browser(NSBrowser, sizeToFitWidthOfColumn: Int) -> CGFloat

Returns the ideal width for a column.

func browserColumnConfigurationDidChange(Notification)

Used by clients to implement their own column width persistence.

func browser(NSBrowser, heightOfRow: Int, inColumn: Int) -> CGFloat

Specifies the height of the specified row in the specified column.

