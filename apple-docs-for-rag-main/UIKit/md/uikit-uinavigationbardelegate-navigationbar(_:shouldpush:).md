

- UIKit
- UINavigationBarDelegate
-  navigationBar(\_:shouldPush:) 

Instance Method

# navigationBar(\_:shouldPush:)

Returns a Boolean value indicating whether the navigation bar should push an item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func navigationBar(
    _ navigationBar: UINavigationBar,
    shouldPush item: UINavigationItem
) -> Bool
```

## Parameters 

`navigationBar`  

The navigation bar that the item is being pushed onto.

`item`  

The navigation item that is being pushed.

## Return Value

true if the item should be pushed; otherwise, false.

## Discussion

Sent to the delegate before pushing an item onto the navigation bar.

## See Also

### Pushing items

func navigationBar(UINavigationBar, didPush: UINavigationItem)

Tells the delegate that an item was pushed onto the navigation bar.

