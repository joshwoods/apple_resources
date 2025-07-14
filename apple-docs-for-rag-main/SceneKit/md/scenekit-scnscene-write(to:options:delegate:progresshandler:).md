

- SceneKit
- SCNScene
-  write(to:options:delegate:progressHandler:) 

Instance Method

# write(to:options:delegate:progressHandler:)

Exports the scene and its contents to a file at the specified URL.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.9+tvOS 10.0+visionOS 1.0+

``` source
func write(
    to url: URL,
    options: [String : Any]? = nil,
    delegate: (any SCNSceneExportDelegate)?,
    progressHandler: SCNSceneExportProgressHandler? = nil
) -> Bool
```

## Parameters 

`url`  

The URL to write the scene file to. This URL must use the `file` scheme.

`options`  

A dictionary of options affecting scene loading, or `nil` for default options. For available keys, see Scene Loading Options.

`delegate`  

A delegate object to customize export of external resources used by the scene. Pass `nil` for default export of external resources.

`progressHandler`  

A block that SceneKit calls repeatedly to report progress of the export operation.

## Return Value

true if exporting the scene was successful; otherwise, false.

## Discussion

The format of the output file depends on OS and argument file extension:

- In iOS 10.0, tvOS 10.0, watchOS 3.0, OS X v10.11, and later versions, specify the `.scn` extension to save a file in SceneKit’s native format. This format supports all features of SceneKit (including physics, constraints, and particle systems), and reading files in this format is faster than importing from other scene file formats.

- In macOS only, specify the `.dae` extension to export in Digital Asset Exchange (DAE) format for use by other apps. Exported DAE files do not contain scene elements specific to SceneKit, such as physics bodies and fields, constraints, and particle systems.

Older versions of iOS and tvOS don’t include the write(to:options:delegate:progressHandler:) method, but you can still produce a file in `.scn` format through SceneKit’s support for the NSSecureCoding protocol. Use the NSKeyedArchiver class to serialize a scene and all its contents, and the NSKeyedUnarchiver class to load an archived scene.

If the scene references external resources, such as image files used in material properties, SceneKit exports these files to a nearby location and references their URLs in the exported scene file. To override SceneKit’s exporting of external resources, provide an object implementing the SCNSceneExportDelegate protocol in the `delegate` parameter.

## See Also

### Exporting a Scene File

protocol SCNSceneExportDelegate

Methods you can implement to participate in the process of exporting a scene to a file.

