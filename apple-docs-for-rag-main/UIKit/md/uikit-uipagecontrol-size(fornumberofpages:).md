

- UIKit
- UIPageControl
-  size(forNumberOfPages:) 

Instance Method

# size(forNumberOfPages:)

Returns the size the receiver’s bounds should be to accommodate the given number of pages.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func size(forNumberOfPages pageCount: Int) -> CGSize
```

## Parameters 

`pageCount`  

The number of pages to fit in the receiver’s bounds.

## Return Value

The minimum size required to display dots for the page count.

## Discussion

Subclasses that customize the appearance of the page control can use this method to resize the page control when the page count changes.

