

- UIKit
- UINavigationBarDelegate
-  navigationBar(\_:shouldPop:) 

Instance Method

# navigationBar(\_:shouldPop:)

Returns a Boolean value indicating whether the navigation bar should pop an item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func navigationBar(
    _ navigationBar: UINavigationBar,
    shouldPop item: UINavigationItem
) -> Bool
```

## Parameters 

`navigationBar`  

The navigation bar that the item is being popped from.

`item`  

The navigation item that is being popped.

## Return Value

true if the item should be popped; otherwise, false.

## Discussion

Sent to the delegate before popping an item from the navigation bar.

## See Also

### Popping items

func navigationBar(UINavigationBar, didPop: UINavigationItem)

Tells the delegate that an item was popped from the navigation bar.

