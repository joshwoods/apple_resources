

- UIKit
- UIWindow
-  makeKey() 

Instance Method

# makeKey()

Makes the window the key window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func makeKey()
```

## Discussion

Use this method to make the window key without changing its visibility. The key window receives keyboard and other non-touch related events. This method causes the previous key window to resign the key status.

## See Also

### Making windows key

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window.

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKeyAndVisible()

Shows the window and makes it the key window.

func becomeKey()

Tells the window that it’s the key window.

func resignKey()

Tells the window that it’s no longer the key window.

