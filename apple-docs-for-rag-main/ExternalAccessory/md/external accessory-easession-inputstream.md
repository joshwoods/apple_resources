

- External Accessory
- EASession
-  inputStream 

Instance Property

# inputStream

The stream to use for receiving data from the accessory.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var inputStream: InputStream? { get }
```

## Discussion

This stream is provided for you automatically by the session object but you must configure it if you want to receive any associated stream events. You do this by assigning a delegate object to the stream that implements the stream(_:handle:) delegate method. You must then schedule the stream in a run loop so that it can receive data asynchronously from one of your application’s threads.

For information on how to schedule an input stream in a run loop and use it to receive data, see Stream Programming Guide.

## See Also

### Getting the Communication Streams

var outputStream: OutputStream?

The stream to use for sending data to the accessory.

