

- File Provider
- NSFileProviderServicing
-  supportedServiceSources(for:completionHandler:) 

Instance Method

# supportedServiceSources(for:completionHandler:)

Asks the File Provider extension for an array of custom communication channels.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func supportedServiceSources(
    for itemIdentifier: NSFileProviderItemIdentifier,
    completionHandler: @escaping ([any NSFileProviderServiceSource]?, (any Error)?) -> Void
) -> Progress
```

**Required**

## Parameters 

`itemIdentifier`  

The item’s identifier.

`completionHandler`  

A block that you call after gathering the service sources. You pass the following parameters:

serviceSources  
An array of service sources that lets you communicate with the host app.

error  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Return Value

An item that tracks the progress of the

## Discussion

The system calls this method when an app requests a list of supported services. Return an array of services for the specified file. An application with access to the file can request the supported services by calling the FileManager class’s getFileProviderServicesForItem(at:completionHandler:) method. For more information, see NSFileProviderService.

