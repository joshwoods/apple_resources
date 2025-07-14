

- AppKit
- NSBrowserDelegate
-  browser(\_:heightOfRow:inColumn:) 

Instance Method

# browser(\_:heightOfRow:inColumn:)

Specifies the height of the specified row in the specified column.

macOS 10.6+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    heightOfRow row: Int,
    inColumn columnIndex: Int
) -> CGFloat
```

## Parameters 

`browser`  

The browser.

`row`  

The index of the row.

`columnIndex`  

The index of the column.

## Return Value

The height to set for the specified row, which must be greater than 0.

## Discussion

The values returned for this method may be cached. Therefore, you should call noteHeightOfRowsWithIndexesChanged(_:inColumn:) to invalidate a row’s height before changing it.

## See Also

### Sizing

func browser(NSBrowser, shouldSizeColumn: Int, forUserResize: Bool, toWidth: CGFloat) -> CGFloat

Used to determine a column’s initial size.

func browser(NSBrowser, sizeToFitWidthOfColumn: Int) -> CGFloat

Returns the ideal width for a column.

func browserColumnConfigurationDidChange(Notification)

Used by clients to implement their own column width persistence.

