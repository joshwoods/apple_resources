

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
- PhotogrammetrySession.Request.Detail
-  PhotogrammetrySession.Request.Detail.custom 

Case

# PhotogrammetrySession.Request.Detail.custom

A custom quality for the model, with specifics defined by the photogrammetry session.

Mac Catalyst 17.0+macOS 14.0+

``` source
case custom
```

## Discussion

If you select `.custom`, you can define unique detail parameters by configuring the session with a PhotogrammetrySession.Configuration.CustomDetailSpecification instance in a customDetailSpecification. The configuration lets you precisely control the model’s detail level, processing efficiency, and output file size by adjusting properties such as maximumPolygonCount, textureFormat, and more.

Note

customDetailSpecification will be applied to every PhotogrammetrySession.Request that specifies a `.custom` detail in this session. It has no effect on the other levels.

