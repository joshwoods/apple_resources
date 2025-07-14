

- SwiftUI
- CommandGroupPlacement
-  systemServices 

Type Property

# systemServices

Placement for commands that expose services other apps provide.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static let systemServices: CommandGroupPlacement
```

## Discussion

By default, this group includes the following command in macOS:

- Services submenu (managed automatically)

## See Also

### App interactions

static let appInfo: CommandGroupPlacement

Placement for commands that provide information about the app, the terms of the user’s license agreement, and so on.

static let appSettings: CommandGroupPlacement

Placement for commands that expose app settings and preferences.

static let appTermination: CommandGroupPlacement

Placement for commands that result in app termination.

static let appVisibility: CommandGroupPlacement

Placement for commands that control the visibility of running apps.

