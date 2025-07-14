

- Group Activities
- SceneAssociationBehavior
-  default 

Type Property

# default

A behavior that matches the activity to a scene using the identifier of your activity object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let `default`: SceneAssociationBehavior
```

## Mentioned in 

Adding spatial Persona support to an activity

## Discussion

With this option, the system uses the string in the activityIdentifier property of your GroupActivity object to locate an appropriate scene. Choose this option if your app has only one scene, or if you always use the same scene to display the intended activity.

## See Also

### Getting the scene-association options

static func content(String) -> SceneAssociationBehavior

A behavior that matches the activity to a scene using a custom string that you supply.

static let none: SceneAssociationBehavior

A behavior that doesn’t match any scenes to the activity.

