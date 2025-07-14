

- WatchKit
- WKInterfaceSlider
-  setValue(\_:) 

Instance Method

# setValue(\_:)

Changes the value of the slider.

watchOS 2.0+

``` source
func setValue(_ value: Float)
```

## Parameters 

`value`  

The new value for the slider. If the new value is outside of the slider’s acceptable range, this method clamps the new value to the minimum or maximum value.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Setting the Slider Value

func setColor(UIColor?)

Sets the color of the slider bar.

func setNumberOfSteps(Int)

Sets the number of steps for the slider.

