

- Automator
- AMAction
-  activated() 

Instance Method

# activated()

Allows the action to synchronize its information with settings in another app.

Mac Catalyst 14.0+macOS 10.4+

``` source
func activated()
```

## Discussion

The system invokes this method when the window of the Automator workflow to which the action belongs becomes the main window.

Be sure to invoke the superclass implementation of this method as the last thing in your implementation.

## See Also

### Initializing and Synchronizing the Action User Interface

func opened()

Allows the action to initialize its user interface.

