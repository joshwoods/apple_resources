

- Foundation
- URLSessionTask
-  resume() 

Instance Method

# resume()

Resumes the task, if it is suspended.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func resume()
```

## Mentioned in 

Uploading streams of data

Downloading files from websites

Pausing and resuming downloads

Pausing and resuming uploads

Fetching website data into memory

## Discussion

Newly-initialized tasks begin in a suspended state, so you need to call this method to start the task.

## See Also

### Controlling the task state

func cancel()

Cancels the task.

func suspend()

Temporarily suspends a task.

var state: URLSessionTask.State

The current state of the task—active, suspended, in the process of being canceled, or completed.

enum State

Constants for determining the current state of a task.

var priority: Float

The relative priority at which you’d like a host to handle the task, specified as a floating point value between `0.0` (lowest priority) and `1.0` (highest priority).

URL session task priority

Constants for providing task priority hints to a host, used with the priority property.

