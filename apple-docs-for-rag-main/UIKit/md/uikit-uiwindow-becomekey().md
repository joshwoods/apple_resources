

- UIKit
- UIWindow
-  becomeKey() 

Instance Method

# becomeKey()

Tells the window that it’s the key window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func becomeKey()
```

## Discussion

Never call this method directly. The system calls this method and posts didBecomeKeyNotification to let the window know that it’s the key window. The default implementation of this method does nothing, but subclasses can override it and use it to perform tasks related to becoming the key window.

In iOS 15 and later, the system calls this method when the window becomes the key window in its scene. In iOS 14 and earlier, the system calls this method when the window becomes the key window in the app.

## See Also

### Making windows key

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window.

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKeyAndVisible()

Shows the window and makes it the key window.

func makeKey()

Makes the window the key window.

func resignKey()

Tells the window that it’s no longer the key window.

