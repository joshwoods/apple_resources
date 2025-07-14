

- Foundation
- ProcessInfo
-  performActivity(options:reason:using:) 

Instance Method

# performActivity(options:reason:using:)

Synchronously perform an activity defined by a given block using the given options.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func performActivity(
    options: ProcessInfo.ActivityOptions = [],
    reason: String,
    using block: @escaping () -> Void
)
```

## Parameters 

`options`  

Options for the activity. See ProcessInfo.ActivityOptions for possible values.

`reason`  

A string used in debugging to indicate the reason the activity began.

`block`  

A block containing the work to be performed by the activity.

## Discussion

The activity will be automatically ended after `block` returns.

## See Also

### Managing Activities

func beginActivity(options: ProcessInfo.ActivityOptions, reason: String) -> any NSObjectProtocol

Begin an activity using the given options and reason.

func endActivity(any NSObjectProtocol)

Ends the given activity.

func performExpiringActivity(withReason: String, using: (Bool) -> Void)

Performs the specified block asynchronously and notifies you if the process is about to be suspended.

