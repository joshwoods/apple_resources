

- Foundation
- App Extension Support
- NSItemProvider
-  Keys for Items Accessed in JavaScript Code 

API Collection

# Keys for Items Accessed in JavaScript Code

Keys in property list items that the system recieves from or sends to JavaScript code.

## Topics

### Constants

let NSExtensionJavaScriptPreprocessingResultsKey: String

A key whose value is an item of type `kUTTypePropertyList`. The item contains an `NSDictionary` that contains the object returned by the JavaScript code to its completion function.

let NSExtensionJavaScriptFinalizeArgumentKey: String

A key whose value is an item of type `kUTTypePropertyList`. The item contains an `NSDictionary` that contains the arguments to be passed to a JavaScript finalize method.

## See Also

### Constants

typealias CompletionHandler

A block that receives the item provider’s data.

typealias LoadHandler

A block that loads the item provider’s data and coerces it to the specified type.

Options Dictionary Key

Keys indicating options to use when generating the item provider’s data.

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

