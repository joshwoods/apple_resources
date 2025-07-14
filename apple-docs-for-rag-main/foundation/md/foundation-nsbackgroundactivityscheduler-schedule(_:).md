

- Foundation
- NSBackgroundActivityScheduler
-  schedule(\_:) 

Instance Method

# schedule(\_:)

Begins scheduling the background activity.

macOS 10.10+

``` source
func schedule(_ block: @escaping (@escaping NSBackgroundActivityScheduler.CompletionHandler) -> Void)
```

## Parameters 

`block`  

A block of code to execute when the scheduler runs. This block will be called on a serial background queue appropriate for the level of quality of service specified. See qualityOfService.

## Discussion

When your block is called, it’s passed a completion handler as an argument. Configure the block to invoke this handler, passing it a result of type NSBackgroundActivityScheduler.Result to indicate whether the activity finished (NSBackgroundActivityScheduler.Result.finished) or should be deferred (NSBackgroundActivityScheduler.Result.deferred) and rescheduled for a later time. Failure to invoke the completion handler results in the activity not being rescheduled. For work that will be deferred and rescheduled, the block may optionally adjust scheduler properties, such as interval or tolerance, before calling the completion handler. See Schedule Activity with scheduleWithBlock:.

## See Also

### Related Documentation

enum Result

These constants indicate whether background activity has been completed successfully or whether additional processing should be deferred until a more optimal time.

### Scheduling Activity

typealias CompletionHandler

