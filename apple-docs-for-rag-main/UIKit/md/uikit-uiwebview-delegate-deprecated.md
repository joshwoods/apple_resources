

- UIKit
- UIWebView
-  delegate Deprecated

Instance Property

# delegate

The receiver’s delegate.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
unowned(unsafe) var delegate: (any UIWebViewDelegate)? { get set }
```

## Discussion

The delegate is sent messages when content is loading. See UIWebViewDelegate for the optional methods this delegate may implement.

Important

Before releasing an instance of `UIWebView` for which you have set a delegate, you must first set its delegate property to `nil`. This can be done, for example, in your dealloc method.

## See Also

### Responding to web view changes

protocol UIWebViewDelegate

The `UIWebViewDelegate` protocol defines methods that a delegate of a UIWebView object can optionally implement to intervene when web content is loaded.

