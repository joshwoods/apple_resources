

- IOUSBHost
- IOUSBHostStream
-  abort(with:) 

Instance Method

# abort(with:)

Aborts pending input/output requests.

Mac Catalyst 14.0+macOS 10.15+

``` source
func abort(with option: IOUSBHostAbortOption) throws
```

## Parameters 

`option`  

A set of options. IOUSBHostAbortOption.synchronous is the default.

## Discussion

Set the stream context as nonactive on the device with an out-of-band (class-defined) mechanism before calling this method, in accordance with USB 3.2, 8.12.1.4. The device won’t select a nonactive stream to become the current stream on the endpoint.

## Topics

### Options

enum IOUSBHostAbortOption

Options for aborting pending input/output requests.

## See Also

### Sending I/O

typealias IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

func enqueueIORequest(with: NSMutableData?, completionHandler: IOUSBHostCompletionHandler?) throws

Enqueues an input/output request on the stream.

func abort() throws

Aborts pending input/output requests synchronously.

