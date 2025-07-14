

- WebKit
-  WKOpenPanelParameters 

Class

# WKOpenPanelParameters

The configuration details of a file upload control in your web content.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.12+

``` source
@MainActor
class WKOpenPanelParameters
```

## Overview

Use a WKOpenPanelParameters to determine the configuration of a file upload control. You don’t create this object directly. Instead, a web view creates one and passes it to the webView(_:runOpenPanelWith:initiatedByFrame:completionHandler:) method of its UI delegate object when it displays a file upload control.

## Topics

### Configuring the panel parameters

var allowsMultipleSelection: Bool

A Boolean value that indicates whether the file upload control supports multiple files.

var allowsDirectories: Bool

A Boolean value that indicates whether the file upload control supports the selection of directories.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Displaying an upload panel

func webView(WKWebView, runOpenPanelWith: WKOpenPanelParameters, initiatedByFrame: WKFrameInfo, completionHandler: ([URL]?) -> Void)

Displays a file upload panel.

