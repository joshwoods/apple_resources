

- Game Controller
- GCVirtualController
-  setPosition(\_:forDirectionPadElement:) 

Instance Method

# setPosition(\_:forDirectionPadElement:)

Changes the value of a directional pad element in the virtual controller.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func setPosition(
    _ position: CGPoint,
    forDirectionPadElement element: String
)
```

## Parameters 

`position`  

A point with `x` and `y` values in the range `[0.0, 1.0]`.

`element`  

The name of the directional pad element to update.

## Discussion

Use this method to update the value of a directional pad in the virtual controller when you set the isHidden property to true and present your own virtual controller interface.

## See Also

### Presenting a custom interface

func setValue(CGFloat, forButtonElement: String)

Changes the value of a button element in the virtual controller.

