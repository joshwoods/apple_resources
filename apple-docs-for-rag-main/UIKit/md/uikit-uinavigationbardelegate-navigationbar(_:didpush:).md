

- UIKit
- UINavigationBarDelegate
-  navigationBar(\_:didPush:) 

Instance Method

# navigationBar(\_:didPush:)

Tells the delegate that an item was pushed onto the navigation bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func navigationBar(
    _ navigationBar: UINavigationBar,
    didPush item: UINavigationItem
)
```

## Parameters 

`navigationBar`  

The navigation bar that the item is being pushed onto.

`item`  

The navigation item that is being pushed.

## Discussion

If pushing an item onto the navigation bar is animated, this method is invoked after the animation ends; otherwise, it is invoked immediately after the push.

## See Also

### Pushing items

func navigationBar(UINavigationBar, shouldPush: UINavigationItem) -> Bool

Returns a Boolean value indicating whether the navigation bar should push an item.

