

- Group Activities
- SystemCoordinator
- SystemCoordinator.Configuration
-  spatialTemplatePreference 

Instance Property

# spatialTemplatePreference

The preferred arrangement of spatial Personas in your app’s immersive space.

visionOS 1.0+

``` source
var spatialTemplatePreference: SpatialTemplatePreference
```

## Discussion

When the system displays spatial Personas, it uses the value of this property to determine how to arrange them around the content in your app’s immersive space. The default value of this property is none , which lets the system determine placement based on the activity’s content. Specify other options if you prefer a specific arrangement around your app’s content.

## See Also

### Specifying spatial position preferences

struct SpatialTemplatePreference

A structure that specifies the preferred arrangement of participant spatial Personas in a shared simulation space.

