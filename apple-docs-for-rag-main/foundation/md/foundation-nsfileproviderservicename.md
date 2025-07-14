

- Foundation
-  NSFileProviderServiceName 

Structure

# NSFileProviderServiceName

The name used to identify a File Provider service.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSFileProviderServiceName
```

## Discussion

The team providing the protocol also defines the name. To create a new service’s name:

- Use reverse domain name notation for the interfaces name (for example, `com.example.MyInterface`).

- (Optional) Incorporate versioning by appending a version number to the end of the name (`com.example.MyInterface.v2`).

For more information on defining a service’s protocol, see Defining the Service’s Protocol.

## Topics

### Initializers

init(String)

Instantiates a new service name from the provided string.

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing File Provider Services

func getFileProviderServicesForItem(at: URL, completionHandler: ([NSFileProviderServiceName : NSFileProviderService]?, (any Error)?) -> Void)

Returns the services provided by the File Provider extension that manages the item at the given URL.

class NSFileProviderService

A service that provides a custom communication channel between your app and a File Provider extension.

