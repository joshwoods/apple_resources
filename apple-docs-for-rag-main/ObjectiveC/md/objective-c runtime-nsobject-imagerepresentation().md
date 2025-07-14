

- Objective-C Runtime
- NSObject
-  imageRepresentation() 

Instance Method

# imageRepresentation()

Returns the image to display.

macOS

``` source
func imageRepresentation() -> Any!
```

## Return Value

The image to display; can return `nil` if the item has no image to display.

## Discussion

Your data source must implement this method. This method is called frequently, so the receiver should cache the returned instance.

