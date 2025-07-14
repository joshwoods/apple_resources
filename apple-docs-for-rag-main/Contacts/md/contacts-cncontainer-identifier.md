

- Contacts
- CNContainer
-  identifier 

Instance Property

# identifier

The unique identifier for a contacts container on the device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var identifier: String { get }
```

## Discussion

It is recommended that you use the identifier when re-fetching the container. The identifier can be persisted between app launches.

## See Also

### Getting the Container Information

var name: String

The name of the container.

var type: CNContainerType

The type of the container.

enum CNContainerType

The container may be local on the device or associated with a server account that has contacts.

