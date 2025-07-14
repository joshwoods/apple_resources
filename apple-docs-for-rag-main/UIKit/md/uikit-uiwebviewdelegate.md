

- UIKit
-  UIWebViewDelegate 

Protocol

# UIWebViewDelegate

The `UIWebViewDelegate` protocol defines methods that a delegate of a UIWebView object can optionally implement to intervene when web content is loaded.

iOSiPadOS

``` source
@MainActor
protocol UIWebViewDelegate : NSObjectProtocol
```

## Overview

Important

Before releasing an instance of `UIWebView` for which you have set a delegate, you must first set the `UIWebView` delegate property to `nil` before disposing of the `UIWebView` instance. This can be done, for example, in the dealloc method where you dispose of the `UIWebView`.

## Topics

### Loading Content

func webView(UIWebView, shouldStartLoadWith: URLRequest, navigationType: UIWebView.NavigationType) -> Bool

Sent before a web view begins loading a frame.

Deprecated

func webViewDidStartLoad(UIWebView)

Sent after a web view starts loading a frame.

Deprecated

func webViewDidFinishLoad(UIWebView)

Sent after a web view finishes loading a frame.

Deprecated

func webView(UIWebView, didFailLoadWithError: any Error)

Sent if a web view failed to load a frame.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to web view changes

var delegate: (any UIWebViewDelegate)?

The receiver’s delegate.

Deprecated

