

- Swift
- Result
- Result.Publisher
-  init(\_:) 

Initializer

# init(\_:)

Creates a publisher that sends the specified output to all subscribers and finishes normally.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ output: Result.Publisher.Output)
```

## Parameters 

`output`  

The output to deliver to each subscriber.

## See Also

### Creating a Result Publisher

init(Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>)

Creates a publisher that delivers the specified result.

init(Failure)

Creates a publisher that immediately terminates upon subscription with the given failure.

