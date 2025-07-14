

- SwiftUI
- WindowManagerRole
-  automatic 

Type Property

# automatic

The automatic role. The type and configuration of the scene will be used to determine how its windows behave in full screen and Stage Manager.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static let automatic: WindowManagerRole
```

## Discussion

On macOS, WindowGroup and DocumentGroup scenes will use the `principal` role. Window scenes will use the `principal` role when they are specified as the first scene in the app’s definition, and use the `associated` role otherwise. Settings will use the `associated` role.

