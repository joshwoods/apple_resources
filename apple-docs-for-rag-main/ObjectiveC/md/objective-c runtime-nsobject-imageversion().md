

- Objective-C Runtime
- NSObject
-  imageVersion() 

Instance Method

# imageVersion()

Returns the version of the item.

macOS

``` source
func imageVersion() -> Int
```

## Return Value

The version of the item.

## Discussion

This method is optional. The receiver can return a new version to let the image browser know that it should not use its cache for the item.

