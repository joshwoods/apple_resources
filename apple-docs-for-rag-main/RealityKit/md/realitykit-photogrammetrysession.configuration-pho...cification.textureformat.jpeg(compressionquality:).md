

- RealityKit
- PhotogrammetrySession
- 
  - PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
- PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat
-  PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat.jpeg(compressionQuality:) 

Case

# PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat.jpeg(compressionQuality:)

Textures will be output in JPG format with the given `compressionQuality` in the range of \[0, 1\], where 1.0 is highest quality (least compression, larger size) and 0.0 is the lowest quality (most compression, smallest size).

Mac Catalyst 17.0+macOS 14.0+

``` source
case jpeg(compressionQuality: Float = 0.8)
```

