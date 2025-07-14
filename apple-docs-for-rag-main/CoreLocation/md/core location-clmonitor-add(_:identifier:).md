

- Core Location
- CLMonitor
-  add(\_:identifier:) 

Instance Method

# add(\_:identifier:)

Adds the given condition for monitoring.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
func add(
    _ Condition: any CLCondition,
    identifier: String
)
```

## Parameters 

`Condition`  

The condition to monitor.

`identifier`  

A string that identifies the monitored condition.

## Discussion

The framework encapsulates the condition in an instance of CLMonitor.Record and then associates the record, along with the condition with the given identifier. The initial state is CLRegionState.unknown.

## See Also

### Adding and removing conditions

func add(any CLCondition, identifier: String, assuming: CLMonitor.Event.State)

Adds the monitoring condition with the identifier and initial state you specify.

func record(for: String) -> CLMonitor.Record?

A record that contains a condition and the most recent event your app receives.

func remove(String)

Removes the condition and its enclosed record associated with the identifier you provide.

