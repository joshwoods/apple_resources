

- WebKit
- WKWebExtension
-  optionalPermissions 

Instance Property

# optionalPermissions

The set of permissions that the extension may need for optional functionality.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var optionalPermissions: Set { get }
```

## Discussion

These permissions can be requested by the extension at a later time.

