

- Group Activities
- SceneAssociationBehavior
-  content(\_:) 

Type Method

# content(\_:)

A behavior that matches the activity to a scene using a custom string that you supply.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static func content(_ contentIdentifier: String) -> SceneAssociationBehavior
```

## Parameters 

`contentIdentifier`  

The string to compare against the scene’s defined activation conditions. This string has a similar purpose to the targetContentIdentifier of an NSUserActivity object.

## Return Value

A SceneAssociationBehavior type with the specified identifier.

## Mentioned in 

Adding spatial Persona support to an activity

## Discussion

Use this option when you want more control over the scene-selection process for your GroupActivity object. You might use it to direct the activity to different scenes, or to direct the activity to a specific instance of a scene. For example, a drawing app might direct the activity to the specific canvas someone wants to share, and not to a new or unrelated canvas that uses the same scene type.

## See Also

### Getting the scene-association options

static let `default`: SceneAssociationBehavior

A behavior that matches the activity to a scene using the identifier of your activity object.

static let none: SceneAssociationBehavior

A behavior that doesn’t match any scenes to the activity.

