

- SceneKit
- SCNSceneSource
-  init(url:options:) 

Initializer

# init(url:options:)

Initializes a scene source for reading the scene graph from a specified file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init?(
    url: URL,
    options: [SCNSceneSource.LoadingOption : Any]? = nil
)
```

## Parameters 

`url`  

The URL identifying the scene.

`options`  

A dictionary containing options that affect scene loading. See `Scene Loading Options` for available keys and values. Pass `nil` to use default options.

## Return Value

An initialized scene source object, or `nil` if initialization was not successful.

## Discussion

If you have the contents of a scene file but not the file itself (for example, if your app downloads scene files from the network), use the init(data:options:) method instead.

## See Also

### Creating a Scene Source

init?(data: Data, options: [SCNSceneSource.LoadingOption : Any]?)

Initializes a scene source for reading the scene graph contained in an `NSData` object.

