

- UIKit
- UIPress
- UIPress.PressType
-  UIPress.PressType.pageDown 

Case

# UIPress.PressType.pageDown

A constant that represents the page down button.

tvOS 14.3+

``` source
case pageDown
```

## Discussion

Add gesture recognizers for UIPress.PressType.pageDown and UIPress.PressType.pageUp to navigate content in your app.

In an electronic program guide, select the item below the current one in response to UIPress.PressType.downArrow, and display the next screen of items in response to UIPress.PressType.pageDown. While your content plays, change the channel when your app receives UIPress.PressType.pageUp or UIPress.PressType.pageDown.

For more details on browsing multichannel content, see Providing Channel Navigation.

## See Also

### Navigation

case upArrow

A constant that represents the up arrow button.

case downArrow

A constant that represents the down arrow button.

case leftArrow

A constant that represents the left arrow button.

case rightArrow

A constant that represents the right arrow button.

case pageUp

A constant that represents the page up button.

