

- Foundation
- URLSession
-  dataTask(with:) 

Instance Method

# dataTask(with:)

Creates a task that retrieves the contents of the specified URL.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dataTask(with url: URL) -> URLSessionDataTask
```

## Parameters 

`url`  

The URL to be retrieved.

## Return Value

The new session data task.

## Mentioned in 

Fetching website data into memory

## Discussion

After you create the task, you must start it by calling its resume() method. The task calls methods on the session’s delegate to provide you with the response metadata, response data, and so on.

## See Also

### Adding data tasks to a session

func dataTask(with: URL, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionDataTask

Creates a task that retrieves the contents of the specified URL, then calls a handler upon completion.

func dataTask(with: URLRequest) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object.

func dataTask(with: URLRequest, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object, and calls a handler upon completion.

class URLSessionDataTask

A URL session task that returns downloaded data directly to the app in memory.

protocol URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

