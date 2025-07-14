

- SceneKit
- SCNSceneSource
-  data 

Instance Property

# data

The data object from which the scene source loads scene content.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data: Data? { get }
```

## Discussion

If the scene source was created using the sceneSourceWithData:options: or init(data:options:) method, this property’s value is the data from which the scene source was created. If the scene source was created from a scene file using the the sceneSourceWithURL:options: or init(url:options:) method, this property’s value is the data loaded from that URL at the time the scene source was created.

## See Also

### Getting Information about the Scene

var url: URL?

The URL identifying the file from which the scene source was created.

func property(forKey: String) -> Any?

Returns metadata about the scene.

