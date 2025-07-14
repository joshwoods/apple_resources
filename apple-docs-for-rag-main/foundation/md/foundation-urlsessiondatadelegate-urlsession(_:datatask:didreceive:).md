

- Foundation
- URLSessionDataDelegate
-  urlSession(\_:dataTask:didReceive:) 

Instance Method

# urlSession(\_:dataTask:didReceive:)

Tells the delegate that the data task has received some of the expected data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    dataTask: URLSessionDataTask,
    didReceive data: Data
)
```

## Parameters 

`session`  

The session containing the data task that provided data.

`dataTask`  

The data task that provided data.

`data`  

A data object containing the transferred data.

## Mentioned in 

Fetching website data into memory

## Discussion

Because the data object parameter is often pieced together from a number of different data objects, whenever possible, use the enumerateBytes(_:) method to iterate through the data rather than using the bytes method (which flattens the data object into a single memory block).

This delegate method may be called more than once, and each call provides only data received since the previous call. The app is responsible for accumulating this data if needed.

