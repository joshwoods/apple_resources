

- SceneKit
-  SCNSceneExportDestinationURL 

Global Variable

# SCNSceneExportDestinationURL

The final destination `URL` for the exported scene file.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
let SCNSceneExportDestinationURL: String
```

## Discussion

Use this option if you export a scene to a temporary directory and then move it to a final location. You must specify a final destination URL (an NSURL object) if your scene references external resources, such as image files for textures. SceneKit uses this URL to construct appropriate paths for external resources when writing the scene file.

