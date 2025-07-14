

- Group Activities
- SpatialTemplatePreference
-  contentExtent(\_:) 

Instance Method

# contentExtent(\_:)

Sets the distance between the app’s content and any participants.

visionOS 1.0+

``` source
func contentExtent(_ contentExtent: CGFloat) -> SpatialTemplatePreference
```

## Mentioned in 

Adding spatial Persona support to an activity

## Discussion

Use this modifier to set the distance between your app’s content and the participants in a shared context. You might use this modifier if the intrinsic size of your content doesn’t represent an optimal viewing distance. Specify the new size in points.

If you don’t apply this modifier, the system uses the intrinsic size of the scene’s content to determine the viewing distance for participants.

