

- Foundation
- ProcessInfo
-  beginActivity(options:reason:) 

Instance Method

# beginActivity(options:reason:)

Begin an activity using the given options and reason.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func beginActivity(
    options: ProcessInfo.ActivityOptions = [],
    reason: String
) -> any NSObjectProtocol
```

## Parameters 

`options`  

Options for the activity. See ProcessInfo.ActivityOptions for possible values.

`reason`  

A string used in debugging to indicate the reason the activity began.

## Return Value

An object token representing the activity.

## Discussion

Indicate completion of the activity by calling endActivity(_:) passing the returned object as the argument.

## See Also

### Managing Activities

func endActivity(any NSObjectProtocol)

Ends the given activity.

func performActivity(options: ProcessInfo.ActivityOptions, reason: String, using: () -> Void)

Synchronously perform an activity defined by a given block using the given options.

func performExpiringActivity(withReason: String, using: (Bool) -> Void)

Performs the specified block asynchronously and notifies you if the process is about to be suspended.

