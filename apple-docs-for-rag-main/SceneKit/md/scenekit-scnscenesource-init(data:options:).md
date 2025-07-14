

- SceneKit
- SCNSceneSource
-  init(data:options:) 

Initializer

# init(data:options:)

Initializes a scene source for reading the scene graph contained in an `NSData` object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init?(
    data: Data,
    options: [SCNSceneSource.LoadingOption : Any]? = nil
)
```

## Parameters 

`data`  

A data object containing a scene file in a format recognized by SceneKit.

`options`  

A dictionary containing options that affect scene loading. See `Scene Loading Options` for available keys and values. Pass `nil` to use default options.

## Return Value

An initialized scene source object, or `nil` if initialization was not successful.

## Discussion

The `data` parameter of this method (an NSData) should contain the same data as directly read from a scene file (such as by using the NSData method dataWithContentsOfURL:). Use this method when you have the contents of a scene file but not the file itself—for example, if your app downloads scene files from the network.

## See Also

### Creating a Scene Source

init?(url: URL, options: [SCNSceneSource.LoadingOption : Any]?)

Initializes a scene source for reading the scene graph from a specified file.

