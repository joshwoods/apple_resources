

- Quartz
- QCView
-  play(\_:) 

Instance Method

# play(\_:)

Plays or pauses a composition in a view.

macOS 10.4+

``` source
@IBAction @MainActor
func play(_ sender: Any!)
```

## Parameters 

`sender`  

The object (such as a button or menu item) sending the message to play the composition. You need to connect the object in the interface to the action.

## Discussion

This method starts rendering a composition if it is not already rendering, pauses a composition that is rendering, or resumes rendering for a composition whose rendering is paused. The method is invoked when the user clicks a button or issues a command from some other user interface element, such as a menu.

## See Also

### Using Interface Builder

func start(Any!)

Starts rendering a composition in a view.

func stop(Any!)

Stops rendering a composition in a view.

