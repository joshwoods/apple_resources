

- UIKit
- UISceneSession
-  UISceneSession.Role 

Structure

# UISceneSession.Role

Constants that indicate the possible roles for a scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
struct Role
```

## Mentioned in 

Presenting content on a connected display

## Topics

### Determining scene roles

static let windowApplication: UISceneSession.Role

A scene that displays interactive windows on the device’s built-in display or an externally connected display.

static let windowExternalDisplay: UISceneSession.Role

A scene that displays noninteractive windows on an externally connected display.

Deprecated

static let windowExternalDisplayNonInteractive: UISceneSession.Role

A scene that displays noninteractive windows on an externally connected display.

static let carTemplateApplication: UISceneSession.Role

A scene that displays interactive content on a CarPlay-enabled vehicle screen.

static let CPTemplateApplicationDashboardSceneSessionRoleApplication: UISceneSession.Role

A scene that displays navigation content on the CarPlay Dashboard.

static let CPTemplateApplicationInstrumentClusterSceneSessionRoleApplication: UISceneSession.Role

A scene that displays navigation content on the CarPlay Instruments Cluster.

### Creating scene roles

init(rawValue: String)

Creates a scene role with the specified raw value.

### Type Properties

static let immersiveSpaceApplication: UISceneSession.Role

static let windowApplicationVolumetric: UISceneSession.Role

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the configuration attributes

var name: String?

The app-specific name assigned to the scene configuration.

var role: UISceneSession.Role

The role assigned to the scene configuration.

