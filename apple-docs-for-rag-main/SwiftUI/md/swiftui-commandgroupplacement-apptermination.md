

- SwiftUI
- CommandGroupPlacement
-  appTermination 

Type Property

# appTermination

Placement for commands that result in app termination.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static let appTermination: CommandGroupPlacement
```

## Discussion

By default, this group includes the following command in macOS:

- Quit App

## See Also

### App interactions

static let appInfo: CommandGroupPlacement

Placement for commands that provide information about the app, the terms of the user’s license agreement, and so on.

static let appSettings: CommandGroupPlacement

Placement for commands that expose app settings and preferences.

static let appVisibility: CommandGroupPlacement

Placement for commands that control the visibility of running apps.

static let systemServices: CommandGroupPlacement

Placement for commands that expose services other apps provide.

