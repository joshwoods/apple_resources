

- Game Controller
- GCButtonElementName
-  backLeftButton(position:) 

Type Method

# backLeftButton(position:)

Returns the name of the back left button at the specified location.

iOS 17.4+iPadOS 17.4+Mac CatalystmacOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
static func backLeftButton(position: Int) -> GCButtonElementName
```

## Parameters 

`position`  

The relative position of the button to the other back left button. Pass `0` for the button nearest to the natural rest position of the person’s finger. Pass `1` for an additional button that requires the person to move their fingers to press if it exists.

## Return Value

The name of the back left button.

## See Also

### Getting extended gamepad back button names

static func backRightButton(position: Int) -> GCButtonElementName

Returns the name of the back right button at the specified location.

