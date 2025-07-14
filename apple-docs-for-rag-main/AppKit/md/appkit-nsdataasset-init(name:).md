

- AppKit
- NSDataAsset
-  init(name:) 

Initializer

# init(name:)

Initializes and returns an object with a reference to the named data asset in an asset catalog.

macOS 10.11+

``` source
convenience init?(name: NSDataAsset.Name)
```

## Parameters 

`name`  

The name of the data set in the asset catalog.

## Return Value

The data asset object for the named data set, or `nil` if the data set is not found.

## Discussion

If there are multiple data files in the named data set, this method returns the one with attributes that most closely match the current device available screen space.

This method looks in the asset catalog, in the main bundle for the named data set.

## See Also

### Initializing the data asset

init?(name: NSDataAsset.Name, bundle: Bundle)

Initializes and returns an object with a reference to the named data asset that’s in an asset catalog in the specified bundle.

