

- Foundation
-  NSItemProviderRepresentationVisibility 

Enumeration

# NSItemProviderRepresentationVisibility

Specifications that control which categories of processes can see an item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum NSItemProviderRepresentationVisibility
```

## Topics

### Enumeration Cases

case all

A representation visibility specification conferring item visibility to all processes.

case group

A representation visibility specification confining item visibility to the app’s app group.

case ownProcess

A representation visibility specification confining item visibility to the app that is the source of the item.

case team

A representation visibility specification confining item visibility to processes created by the app’s development team.

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

enum ErrorCode

The error codes that describe problems with consuming data from an item provider.

