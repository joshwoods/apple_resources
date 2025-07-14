

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  customDetailSpecification 

Instance Property

# customDetailSpecification

Defines custom detail level specifications for a photogrammetry session with custom detail level.

Mac Catalyst 17.0+macOS 14.0+

``` source
var customDetailSpecification: PhotogrammetrySession.Configuration.CustomDetailSpecification
```

## Discussion

This property configures the characteristics of the model’s precision and characteristics, such as texture size and the types of texture maps.

Important

The system checks this property only when processing a request with the PhotogrammetrySession.Request.Detail.custom detail set.

