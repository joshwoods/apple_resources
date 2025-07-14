

- Background Tasks
- BGTaskScheduler
-  getPendingTaskRequests(completionHandler:) 

Instance Method

# getPendingTaskRequests(completionHandler:)

Request a list of unexecuted scheduled task requests.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func getPendingTaskRequests(completionHandler: @escaping ([BGTaskRequest]) -> Void)
```

``` source
func pendingTaskRequests() async -> [BGTaskRequest]
```

## Parameters 

`completionHandler`  

The completion handler called with the pending tasks. The handler may execute on a background thread.

The handler takes a single parameter `tasksRequests`, an array of `BGTaskRequest` objects. The array is empty if there are no scheduled tasks.

The objects passed in the array are copies of the existing requests. Changing the attributes of a request has no effect. To change the attributes submit a new task request using submit(_:).

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

