

- Core Location
- CLMonitor
-  record(for:) 

Instance Method

# record(for:)

A record that contains a condition and the most recent event your app receives.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
func record(for identifier: String) -> CLMonitor.Record?
```

## Parameters 

`identifier`  

A string that identifies the monitored condition.

## Return Value

Returns a CLMonitor.Record, or `nil` if the system can’t find the identifier.

## See Also

### Adding and removing conditions

func add(any CLCondition, identifier: String)

Adds the given condition for monitoring.

func add(any CLCondition, identifier: String, assuming: CLMonitor.Event.State)

Adds the monitoring condition with the identifier and initial state you specify.

func remove(String)

Removes the condition and its enclosed record associated with the identifier you provide.

