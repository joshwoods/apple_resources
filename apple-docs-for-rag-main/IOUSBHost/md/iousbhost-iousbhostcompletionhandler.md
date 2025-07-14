

- IOUSBHost
-  IOUSBHostCompletionHandler 

Type Alias

# IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

Mac Catalyst 14.0+macOS 10.15+

``` source
typealias IOUSBHostCompletionHandler = (IOReturn, Int) -> Void
```

## Parameters 

`status`  

The result for the transfer.

`bytesTransferred`  

The number of bytes the request transferred.

