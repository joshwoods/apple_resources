

- UIKit
- UINavigationBarDelegate
-  navigationBar(\_:didPop:) 

Instance Method

# navigationBar(\_:didPop:)

Tells the delegate that an item was popped from the navigation bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func navigationBar(
    _ navigationBar: UINavigationBar,
    didPop item: UINavigationItem
)
```

## Parameters 

`navigationBar`  

The navigation bar that the item is being popped from.

`item`  

The navigation item that is being popped.

## Discussion

If animating the pop operation, this method is invoked after the animation ends; otherwise, it is invoked immediately after the pop.

## See Also

### Popping items

func navigationBar(UINavigationBar, shouldPop: UINavigationItem) -> Bool

Returns a Boolean value indicating whether the navigation bar should pop an item.

