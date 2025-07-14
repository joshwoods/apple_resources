

- UIKit
- UIPageViewControllerDataSource
-  presentationIndex(for:) 

Instance Method

# presentationIndex(for:)

Returns the index of the selected item to be reflected in the page indicator.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func presentationIndex(for pageViewController: UIPageViewController) -> Int
```

## Parameters 

`pageViewController`  

The page view controller.

## Return Value

The index of the selected item to be reflected in the page indicator.

## See Also

### Supporting a Page Indicator

func presentationCount(for: UIPageViewController) -> Int

Returns the number of items to be reflected in the page indicator.

