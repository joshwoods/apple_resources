

- SceneKit
- SCNSceneSource
-  property(forKey:) 

Instance Method

# property(forKey:)

Returns metadata about the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func property(forKey key: String) -> Any?
```

## Parameters 

`key`  

A constant identifying a metadata property of the scene source. See Scene Source Properties for available keys and the formats of their values.

## Return Value

The value for the metadata property, or `nil` if no value exists for the specified property.

## Discussion

This method returns information about the scene that is defined in the file but is not directly referenced by the scene.

## See Also

### Getting Information about the Scene

var url: URL?

The URL identifying the file from which the scene source was created.

var data: Data?

The data object from which the scene source loads scene content.

