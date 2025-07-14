

- UIKit
- UISceneSession
- UISceneSession.Role
-  windowExternalDisplay Deprecated

Type Property

# windowExternalDisplay

A scene that displays noninteractive windows on an externally connected display.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedtvOS 13.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let windowExternalDisplay: UISceneSession.Role
```

Deprecated

Use windowExternalDisplayNonInteractive for a scene that displays noninteractive windows on an externally connected screen. A scene that displays interactive windows uses windowApplication, even if the windows display on an externally connected screen.

## See Also

### Determining scene roles

static let windowApplication: UISceneSession.Role

A scene that displays interactive windows on the device’s built-in display or an externally connected display.

static let windowExternalDisplayNonInteractive: UISceneSession.Role

A scene that displays noninteractive windows on an externally connected display.

static let carTemplateApplication: UISceneSession.Role

A scene that displays interactive content on a CarPlay-enabled vehicle screen.

static let CPTemplateApplicationDashboardSceneSessionRoleApplication: UISceneSession.Role

A scene that displays navigation content on the CarPlay Dashboard.

static let CPTemplateApplicationInstrumentClusterSceneSessionRoleApplication: UISceneSession.Role

A scene that displays navigation content on the CarPlay Instruments Cluster.

