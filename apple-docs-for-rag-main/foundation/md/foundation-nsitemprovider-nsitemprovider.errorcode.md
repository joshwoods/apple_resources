

- Foundation
- NSItemProvider
-  NSItemProvider.ErrorCode 

Enumeration

# NSItemProvider.ErrorCode

The error codes that describe problems with consuming data from an item provider.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum ErrorCode
```

## Topics

### Constants

case itemUnavailableError

An error code indicating that the requested data was unavailable from an item provider.

case unavailableCoercionError

An error code indicating that the requested data type coercion is unavailable from an item provider.

case unexpectedValueClassError

An error code indicating that type coercion to the requested class failed.

case unknownError

An error code indicating an unknown error with consuming data from an item provider.

case itemUnavailableError

An error code indicating that the requested data was unavailable from an item provider.

case unavailableCoercionError

An error code indicating that the requested data type coercion is unavailable from an item provider.

case unexpectedValueClassError

An error code indicating that type coercion to the requested class failed.

case unknownError

An error code indicating an unknown error with consuming data from an item provider.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

typealias CompletionHandler

A block that receives the item provider’s data.

typealias LoadHandler

A block that loads the item provider’s data and coerces it to the specified type.

Options Dictionary Key

Keys indicating options to use when generating the item provider’s data.

Keys for Items Accessed in JavaScript Code

Keys in property list items that the system recieves from or sends to JavaScript code.

class let errorDomain: String

The error domain associated with the item provider.

struct NSItemProviderFileOptions

Data-access specifications that declare how to handle items.

protocol NSItemProviderReading

The protocol for implementing a class to allow an item provider to create an instance of the class.

protocol NSItemProviderWriting

The protocol for implementing a class to allow an item provider to retrieve data from an instance of the class.

enum NSItemProviderRepresentationVisibility

Specifications that control which categories of processes can see an item.

