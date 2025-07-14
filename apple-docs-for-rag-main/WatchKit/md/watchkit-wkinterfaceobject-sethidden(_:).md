

- WatchKit
- WKInterfaceObject
-  setHidden(\_:) 

Instance Method

# setHidden(\_:)

Hides or shows the interface object in your user interface.

watchOS 2.0+

``` source
func setHidden(_ hidden: Bool)
```

## Parameters 

`hidden`  

A Boolean value indicating the visibility of the object. Specify true to hide the object. Specify false to show it.

## Mentioned in 

Connecting Your User Interface to Your Code

## Discussion

When you hide or show an object in your interface, WatchKit makes a note to update the layout during the next refresh cycle. During that cycle, WatchKit adjusts the layout to display only the currently visible objects.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Hiding and Showing an Object

func setAlpha(CGFloat)

Sets the opacity of the interface object.

