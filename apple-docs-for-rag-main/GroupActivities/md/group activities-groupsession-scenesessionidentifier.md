

- Group Activities
- GroupSession
-  sceneSessionIdentifier 

Instance Property

# sceneSessionIdentifier

The persistent identifier of the session’s associated scene.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
final var sceneSessionIdentifier: String? { get }
```

## Discussion

Use this property to determine which of your app’s scenes belongs with this session. You can configure a GroupActivity object with a SceneAssociationBehavior type that tells the system how to associate the activity with one of your app’s scenes. After matching the activity to a specific scene, the system places the scene identifier in this property.

