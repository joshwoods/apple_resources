

- Quartz
- QCView
-  stop(\_:) 

Instance Method

# stop(\_:)

Stops rendering a composition in a view.

macOS 10.4+

``` source
@IBAction @MainActor
func stop(_ sender: Any!)
```

## Parameters 

`sender`  

The object (such as a button or menu item) sending the message to stop rendering. You need to connect the object in the interface to the action.

## Discussion

The method is invoked when the user clicks a button or issues a command from some other user interface element, such as a menu. It is equivalent to the stopRendering() method.

## See Also

### Using Interface Builder

func play(Any!)

Plays or pauses a composition in a view.

func start(Any!)

Starts rendering a composition in a view.

