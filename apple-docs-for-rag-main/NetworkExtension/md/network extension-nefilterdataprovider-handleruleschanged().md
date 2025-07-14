

- Network Extension
- NEFilterDataProvider
-  handleRulesChanged() 

Instance Method

# handleRulesChanged()

Handle a rules changed event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func handleRulesChanged()
```

## Discussion

The system calls this method when the Filter Control Provider calls the `notifyRulesChanged` method or returns a NEFilterControlVerdict with the updateRules() property set to YES.

