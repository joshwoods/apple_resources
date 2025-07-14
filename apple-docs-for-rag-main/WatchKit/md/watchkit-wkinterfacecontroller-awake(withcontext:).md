

- WatchKit
- WKInterfaceController
-  awake(withContext:) 

Instance Method

# awake(withContext:)

Initializes the interface controller with the specified context data.

watchOS 2.0+

``` source
@MainActor
func awake(withContext context: Any?)
```

## Parameters 

`context`  

The context object (if any) provided by the previous interface controller. This parameter may be `nil`. If it is not `nil`, you are responsible for saving a reference to the provided object and using it to configure your interface controller.

## Mentioned in 

Navigating Between Scenes

Working with the watchOS app life cycle

## Discussion

The system calls this method at initialization time to provide the interface controller with any relevant contextual data from a previous interface controller. Use this method to finish the initialization of your interface. For example, you might use this method to load data and to set the values for labels, images, tables, and other interface objects in your storyboard scene. If context data is available, use it to assist in the configuration of the new interface controller.

The default implementation of this method does nothing.

## See Also

### Creating the interface controller

init()

Returns an initialized interface controller object.

func setTitle(String?)

Sets the title of the interface.

