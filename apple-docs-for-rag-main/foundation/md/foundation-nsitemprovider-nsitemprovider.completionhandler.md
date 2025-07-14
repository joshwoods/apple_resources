

- Foundation
- NSItemProvider
-  NSItemProvider.CompletionHandler 

Type Alias

# NSItemProvider.CompletionHandler

A block that receives the item provider’s data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias CompletionHandler = ((any NSSecureCoding)?, (any Error)?) -> Void
```

## Discussion

Use this block to receive data from a call to the loadItem(forTypeIdentifier:options:completionHandler:) method. This block takes the following parameters:

item  
The item to be loaded. When specifying your block, set the type of this parameter to the specific data type you want. For example, when requesting text data, you might set the type to NSString or NSAttributedString. The item provider attempts to coerce the data to the class you specify.

error  
A pointer to an error object for receiving information about any problems that occurred when loading the data.

## See Also

### Constants

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

enum ErrorCode

The error codes that describe problems with consuming data from an item provider.

