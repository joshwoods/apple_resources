

- WatchKit
- WKInterfaceSlider
-  setColor(\_:) 

Instance Method

# setColor(\_:)

Sets the color of the slider bar.

watchOS 2.0+

``` source
func setColor(_ color: UIColor?)
```

## Parameters 

`color`  

The custom color to be applied to the slider bar. Specifying `nil` removes the custom color and returns the slider to the color specified in the storyboard file. The default slider bar color is green.

## See Also

### Setting the Slider Value

func setValue(Float)

Changes the value of the slider.

func setNumberOfSteps(Int)

Sets the number of steps for the slider.

