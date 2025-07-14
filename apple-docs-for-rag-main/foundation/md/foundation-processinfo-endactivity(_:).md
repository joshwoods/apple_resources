

- Foundation
- ProcessInfo
-  endActivity(\_:) 

Instance Method

# endActivity(\_:)

Ends the given activity.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func endActivity(_ activity: any NSObjectProtocol)
```

## Parameters 

`activity`  

An activity object returned by beginActivity(options:reason:).

## See Also

### Managing Activities

func beginActivity(options: ProcessInfo.ActivityOptions, reason: String) -> any NSObjectProtocol

Begin an activity using the given options and reason.

func performActivity(options: ProcessInfo.ActivityOptions, reason: String, using: () -> Void)

Synchronously perform an activity defined by a given block using the given options.

func performExpiringActivity(withReason: String, using: (Bool) -> Void)

Performs the specified block asynchronously and notifies you if the process is about to be suspended.

