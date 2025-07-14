

- SceneKit
- SCNSceneSource
-  url 

Instance Property

# url

The URL identifying the file from which the scene source was created.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var url: URL? { get }
```

## Discussion

The value of this property is `nil` if the scene source was not created using the sceneSourceWithURL:options: or init(url:options:) method.

## See Also

### Getting Information about the Scene

var data: Data?

The data object from which the scene source loads scene content.

func property(forKey: String) -> Any?

Returns metadata about the scene.

