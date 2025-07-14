

- WebKit
- WKWebExtension
- WKWebExtension.Action
-  presentsPopup 

Instance Property

# presentsPopup

A Boolean value indicating whether the action has a pop-up.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var presentsPopup: Bool { get }
```

## Discussion

Use this property to check if the action has a pop-up before attempting to show any pop-up views.

