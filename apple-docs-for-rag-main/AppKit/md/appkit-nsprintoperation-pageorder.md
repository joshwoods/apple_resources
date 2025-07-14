

- AppKit
- NSPrintOperation
-  pageOrder 

Instance Property

# pageOrder

The print order for the pages of the operation.

macOS

``` source
@MainActor
var pageOrder: NSPrintOperation.PageOrder { get set }
```

## Parameters 

`order`  

The print order. For a list of possible values, see NSPrintOperation.PageOrder.

## See Also

### Managing Page Information

var currentPage: Int

The current page number being printed.

var pageRange: NSRange

The range of pages associated with the print operation.

enum PageOrder

Constants that specify the page order.

