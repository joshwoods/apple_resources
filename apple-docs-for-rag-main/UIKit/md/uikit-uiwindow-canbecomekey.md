

- UIKit
- UIWindow
-  canBecomeKey 

Instance Property

# canBecomeKey

A Boolean value that indicates whether the window can become the key window.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var canBecomeKey: Bool { get }
```

## Discussion

The default value is true. To indicate that the window can’t become the key window, override canBecomeKey and return false.

## See Also

### Making windows key

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window.

func makeKeyAndVisible()

Shows the window and makes it the key window.

func makeKey()

Makes the window the key window.

func becomeKey()

Tells the window that it’s the key window.

func resignKey()

Tells the window that it’s no longer the key window.

