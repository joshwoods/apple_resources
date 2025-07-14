

- UIKit
- NSDataAsset
-  init(name:bundle:) 

Initializer

# init(name:bundle:)

Initializes and returns an object with a reference to the named data asset that’s in an asset catalog in the specified bundle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    name: NSDataAssetName,
    bundle: Bundle
)
```

## Parameters 

`name`  

The name of the data set in the asset catalog.

`bundle`  

The bundle used to store the asset catalog. Pass `nil` for the main bundle. The bundle must be the same as the one used in the Xcode project.

## Return Value

The data asset object for the named data set in the specified bundle, or `nil` if the data set is not found.

## Discussion

If there are multiple data files in the named data set, this method returns the one with attributes that most closely match the current device available screen space.

This method looks in the asset catalog, in the bundle specified by the `bundle` parameter for the named data set.

## See Also

### Initializing the data asset

convenience init?(name: NSDataAssetName)

Initializes and returns an object with a reference to the named data asset in an asset catalog.

