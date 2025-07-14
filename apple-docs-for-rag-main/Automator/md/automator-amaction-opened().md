

- Automator
- AMAction
-  opened() 

Instance Method

# opened()

Allows the action to initialize its user interface.

Mac Catalyst 14.0+macOS 10.4+

``` source
func opened()
```

## Discussion

The system invokes this method when the action is first added to a workflow.

You should perform all initializations of an action’s user interface in this method and not in `awakeFromNib`. Be sure to invoke the superclass implementation of this method as the final step of your implementation.

## See Also

### Initializing and Synchronizing the Action User Interface

func activated()

Allows the action to synchronize its information with settings in another app.

