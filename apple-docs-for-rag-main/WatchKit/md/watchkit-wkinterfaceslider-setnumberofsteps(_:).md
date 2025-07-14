

- WatchKit
- WKInterfaceSlider
-  setNumberOfSteps(\_:) 

Instance Method

# setNumberOfSteps(\_:)

Sets the number of steps for the slider.

watchOS 2.0+

``` source
func setNumberOfSteps(_ numberOfSteps: Int)
```

## Parameters 

`numberOfSteps`  

The number of steps between the minimum and maximum value. If the slider’s value is continuous, calling this method has no effect.

## Discussion

Each tap on the slider’s increment or decrement areas changes the slider value by one step. The value of each step is equal to the difference between the minimum and maximum values divided by the number of steps. For example, if the minimum value is `0`, the maximum value is `1`, and the number of steps is `10`, each step increments or decrements the value by `0.1`.

## See Also

### Setting the Slider Value

func setValue(Float)

Changes the value of the slider.

func setColor(UIColor?)

Sets the color of the slider bar.

