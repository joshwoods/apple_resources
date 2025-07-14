

- SceneKit
- SCNScene
-  init(url:options:) 

Initializer

# init(url:options:)

Loads a scene from the specified URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    url: URL,
    options: [SCNSceneSource.LoadingOption : Any]? = nil
) throws
```

## Parameters 

`url`  

The URL to the scene file to load.

`options`  

A dictionary of options affecting scene loading, or `nil` for default options. For available keys, see Scene Loading Options.

## Return Value

A new scene object, or `nil` if no scene could be loaded.

## Discussion

This method provides a convenient way to load a complete scene from a file at an arbitrary URL. For more detailed options or to load only part of a file’s scene graph, use the SCNSceneSource class.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

When creating a scene using Xcode’s Scene Editor or an external tool, you should copy your scene file into a directory with the .scnassets extension inside your app bundle. You should also place any image files referenced as textures from that scene in an Asset Catalog. Xcode will optimize the scene and texture resources for best performance on each target device, and prepare your texture resources for delivery features such as App Thinning and On-Demand Resources.

## See Also

### Creating a Scene from a File

convenience init?(named: String)

Loads a scene from a file with the specified name in the app’s main bundle.

convenience init?(named: String, inDirectory: String?, options: [SCNSceneSource.LoadingOption : Any]?)

Loads a scene from a file with the specified name in a specific subdirectory of the app’s main bundle.

