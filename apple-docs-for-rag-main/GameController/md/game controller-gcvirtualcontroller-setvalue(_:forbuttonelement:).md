

- Game Controller
- GCVirtualController
-  setValue(\_:forButtonElement:) 

Instance Method

# setValue(\_:forButtonElement:)

Changes the value of a button element in the virtual controller.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func setValue(
    _ value: CGFloat,
    forButtonElement element: String
)
```

## Parameters 

`value`  

A value in the range `[-1.0, 1.0]`.

`element`  

The name of the button element to update.

## Discussion

Use this method to update the value of a button element in the virtual controller when you set the isHidden property to true and present your own virtual controller interface.

## See Also

### Presenting a custom interface

func setPosition(CGPoint, forDirectionPadElement: String)

Changes the value of a directional pad element in the virtual controller.

