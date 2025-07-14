

- UIKit
- UIWindow
-  makeKeyAndVisible() 

Instance Method

# makeKeyAndVisible()

Shows the window and makes it the key window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func makeKeyAndVisible()
```

## Discussion

This is a convenience method to show the current window and position it in front of all other windows at the same level or lower. If you only want to show the window, change its isHidden property to false.

## See Also

### Making windows key

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window.

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKey()

Makes the window the key window.

func becomeKey()

Tells the window that it’s the key window.

func resignKey()

Tells the window that it’s no longer the key window.

