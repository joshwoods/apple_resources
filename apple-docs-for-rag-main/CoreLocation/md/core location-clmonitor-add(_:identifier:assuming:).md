

- Core Location
- CLMonitor
-  add(\_:identifier:assuming:) 

Instance Method

# add(\_:identifier:assuming:)

Adds the monitoring condition with the identifier and initial state you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
func add(
    _ condition: any CLCondition,
    identifier: String,
    assuming state: CLMonitor.Event.State
)
```

## Parameters 

`condition`  

The condition to monitor.

`identifier`  

A string that identifies the monitored condition.

`state`  

The monitoring state to initialize the condition with.

## See Also

### Adding and removing conditions

func add(any CLCondition, identifier: String)

Adds the given condition for monitoring.

func record(for: String) -> CLMonitor.Record?

A record that contains a condition and the most recent event your app receives.

func remove(String)

Removes the condition and its enclosed record associated with the identifier you provide.

