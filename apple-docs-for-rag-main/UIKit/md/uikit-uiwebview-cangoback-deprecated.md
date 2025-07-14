

- UIKit
- UIWebView
-  canGoBack Deprecated

Instance Property

# canGoBack

A Boolean value indicating whether the receiver can move backward.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
var canGoBack: Bool { get }
```

## Discussion

If true, able to move backward; otherwise, false.

## See Also

### Moving back and forward

var canGoForward: Bool

A Boolean value indicating whether the receiver can move forward.

Deprecated

func goBack()

Loads the previous location in the back-forward list.

Deprecated

func goForward()

Loads the next location in the back-forward list.

Deprecated

