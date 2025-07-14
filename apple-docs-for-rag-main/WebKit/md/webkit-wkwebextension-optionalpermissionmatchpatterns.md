

- WebKit
- WKWebExtension
-  optionalPermissionMatchPatterns 

Instance Property

# optionalPermissionMatchPatterns

The set of websites that the extension may need access to for optional functionality.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var optionalPermissionMatchPatterns: Set { get }
```

## Discussion

These match patterns can be requested by the extension at a later time.

