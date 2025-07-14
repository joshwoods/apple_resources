

- Automator
- AMAction
-  closed() 

Instance Method

# closed()

Invoked by Automator when the receiving action is removed from a workflow, allowing it to perform cleanup operations.

Mac Catalyst 14.0+macOS 10.5+

``` source
func closed()
```

## Discussion

This method is intended to be overridden, so that your action can perform its specific cleanup operations.

