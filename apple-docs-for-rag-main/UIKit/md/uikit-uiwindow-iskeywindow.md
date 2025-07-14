

- UIKit
- UIWindow
-  isKeyWindow 

Instance Property

# isKeyWindow

A Boolean value that indicates whether the window is the key window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isKeyWindow: Bool { get }
```

## Discussion

In iOS 15 and later, the value of this property is true when the window is the key window of its scene. In iOS 14 and earlier, the value of this property is true when the window is the key window in the app.

The key window receives keyboard and other non-touch-related events. Only one window at a time may be the key window.

## See Also

### Making windows key

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKeyAndVisible()

Shows the window and makes it the key window.

func makeKey()

Makes the window the key window.

func becomeKey()

Tells the window that it’s the key window.

func resignKey()

Tells the window that it’s no longer the key window.

