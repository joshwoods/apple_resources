

- UIKit
- UIPrintFormatter
-  pageCount 

Instance Property

# pageCount

The number of pages to print.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var pageCount: Int { get }
```

## Discussion

`UIPrintFormatter` calculates this value based on the layout metrics and content.

## See Also

### Managing pagination

var startPage: Int

The index of the first page that the print formatter lays out.

