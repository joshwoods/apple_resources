

- SceneKit
- SCNScene
-  init(named:) 

Initializer

# init(named:)

Loads a scene from a file with the specified name in the app’s main bundle.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
convenience init?(named name: String)
```

## Parameters 

`name`  

The name of a scene file in the app bundle’s resources directory.

## Return Value

A new scene object, or `nil` if no scene could be loaded.

## Discussion

This method provides a convenient way to load a complete scene from a file in the app’s main bundle. Calling this method is equivalent to using the Bundle class to locate the scene file and passing the resulting URL to the init(url:options:) method, specifying no options and no error handling.

For more detailed options or to load only part of a file’s scene graph, use the SCNSceneSource class.

When creating a scene using Xcode’s Scene Editor or an external tool, you should copy your scene file into a directory with the .scnassets extension inside your app bundle. You should also place any image files referenced as textures from that scene in an Asset Catalog. Xcode will optimize the scene and texture resources for best performance on each target device, and prepare your texture resources for delivery features such as App Thinning and On-Demand Resources.

## See Also

### Creating a Scene from a File

convenience init?(named: String, inDirectory: String?, options: [SCNSceneSource.LoadingOption : Any]?)

Loads a scene from a file with the specified name in a specific subdirectory of the app’s main bundle.

convenience init(url: URL, options: [SCNSceneSource.LoadingOption : Any]?) throws

Loads a scene from the specified URL.

