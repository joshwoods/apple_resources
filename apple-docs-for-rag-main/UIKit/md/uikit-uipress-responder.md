

- UIKit
- UIPress
-  responder 

Instance Property

# responder

A responder object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var responder: UIResponder? { get }
```

## Discussion

This property is a UIResponder object that either is focused or is the isFirstResponder object in the window when UIApplication originally dispatched the press event.

