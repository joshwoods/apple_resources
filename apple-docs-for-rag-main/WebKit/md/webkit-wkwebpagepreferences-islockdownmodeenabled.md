

- WebKit
- WKWebpagePreferences
-  isLockdownModeEnabled 

Instance Property

# isLockdownModeEnabled

A Boolean value that indicates whether to use Lockdown Mode in the web view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor
var isLockdownModeEnabled: Bool { get set }
```

## Discussion

By default, this reflects whether the user has enabled Lockdown Mode on the device. Update this preference to override the device setting when you implement a per-website or similar setting.

For more information about Lockdown Mode, see About Lockdown Mode.

