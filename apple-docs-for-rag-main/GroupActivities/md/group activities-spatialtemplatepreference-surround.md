

- Group Activities
- SpatialTemplatePreference
-  surround 

Type Property

# surround

An arrangement where the participants sit around the content.

visionOS 2.0+

``` source
static let surround: SpatialTemplatePreference
```

## Discussion

This arrangement works best when the content is 3D, because each participant views it from a different angle

For example:

```
         A

    B   App   D

         C
```

Important

This preference will only apply if your app is using a shared volume or an immersive space with no shared window.

If this preference is applied in an unsupported scenario, like when an app is sharing a window, the system will behave as if the none preference was selected.

