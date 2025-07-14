

- Quartz
- QCView
-  start(\_:) 

Instance Method

# start(\_:)

Starts rendering a composition in a view.

macOS 10.4+

``` source
@IBAction @MainActor
func start(_ sender: Any!)
```

## Parameters 

`sender`  

The object (such as a button or menu item) sending the message to start rendering. You need to connect the object in the interface to the action.

## Discussion

The method is invoked when the user clicks a button or issues a command from some other user interface element, such as a menu. It is equivalent to the startRendering() method.

## See Also

### Using Interface Builder

func play(Any!)

Plays or pauses a composition in a view.

func stop(Any!)

Stops rendering a composition in a view.

