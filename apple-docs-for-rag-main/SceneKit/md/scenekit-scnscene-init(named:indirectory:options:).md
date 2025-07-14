

- SceneKit
- SCNScene
-  init(named:inDirectory:options:) 

Initializer

# init(named:inDirectory:options:)

Loads a scene from a file with the specified name in a specific subdirectory of the app’s main bundle.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init?(
    named name: String,
    inDirectory directory: String?,
    options: [SCNSceneSource.LoadingOption : Any]? = nil
)
```

## Parameters 

`name`  

The name of a scene file in the app bundle.

`directory`  

The path to the subdirectory of the bundle’s resources directory containing the scene file.

`options`  

A dictionary of options affecting scene loading, or `nil` for default options. For available keys, see Scene Loading Options.

## Return Value

A new scene object, or `nil` if no scene could be loaded.

## Discussion

This method provides a convenient way to load a complete scene from a file in the app’s main bundle. Calling this method is equivalent to using the Bundle class to locate the scene file and passing the resulting URL to the init(url:options:) method.

For more detailed options or to load only part of a file’s scene graph, use the SCNSceneSource class.

When creating a scene using Xcode’s Scene Editor or an external tool, you should copy your scene file into a directory with the .scnassets extension inside your app bundle. You should also place any image files referenced as textures from that scene in an Asset Catalog. Xcode will optimize the scene and texture resources for best performance on each target device, and prepare your texture resources for delivery features such as App Thinning and On-Demand Resources.

## See Also

### Creating a Scene from a File

convenience init?(named: String)

Loads a scene from a file with the specified name in the app’s main bundle.

convenience init(url: URL, options: [SCNSceneSource.LoadingOption : Any]?) throws

Loads a scene from the specified URL.

