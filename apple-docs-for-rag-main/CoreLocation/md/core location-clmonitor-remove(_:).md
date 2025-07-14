

- Core Location
- CLMonitor
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the condition and its enclosed record associated with the identifier you provide.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
func remove(_ identifier: String)
```

## Parameters 

`identifier`  

A string that identifies the monitored condition.

## See Also

### Adding and removing conditions

func add(any CLCondition, identifier: String)

Adds the given condition for monitoring.

func add(any CLCondition, identifier: String, assuming: CLMonitor.Event.State)

Adds the monitoring condition with the identifier and initial state you specify.

func record(for: String) -> CLMonitor.Record?

A record that contains a condition and the most recent event your app receives.

