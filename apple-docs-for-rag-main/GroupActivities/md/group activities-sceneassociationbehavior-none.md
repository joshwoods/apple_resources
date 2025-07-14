

- Group Activities
- SceneAssociationBehavior
-  none 

Type Property

# none

A behavior that doesn’t match any scenes to the activity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let none: SceneAssociationBehavior
```

## Mentioned in 

Adding spatial Persona support to an activity

## Discussion

Choose this option when you don’t want the system to associate one of your scenes with the SharePlay activity. You might choose this option when you handle an activity separately from your app’s scenes.

## See Also

### Getting the scene-association options

static let `default`: SceneAssociationBehavior

A behavior that matches the activity to a scene using the identifier of your activity object.

static func content(String) -> SceneAssociationBehavior

A behavior that matches the activity to a scene using a custom string that you supply.

