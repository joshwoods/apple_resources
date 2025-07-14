

- Swift
- Result
- Result.Publisher
-  init(\_:) 

Initializer

# init(\_:)

Creates a publisher that delivers the specified result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ result: Result.Publisher.Output, Failure>)
```

## Parameters 

`result`  

The result to deliver to each subscriber.

## Discussion

If `result` is `Swift/Result/success`, then the publisher waits until it receives a request for at least one value, then sends the output to all subscribers and finishes normally. If `result` is `Swift/Result/failure`, then the publisher sends the failure immediately upon subscription.

## See Also

### Creating a Result Publisher

init(Failure)

Creates a publisher that immediately terminates upon subscription with the given failure.

init(Result&lt;Success, Failure>.Publisher.Output)

Creates a publisher that sends the specified output to all subscribers and finishes normally.

