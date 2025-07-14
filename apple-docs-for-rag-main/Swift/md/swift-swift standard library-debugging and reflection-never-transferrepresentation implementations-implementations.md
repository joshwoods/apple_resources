

- Swift
- Swift Standard Library
- Debugging and Reflection
- Never
-  TransferRepresentation Implementations 

API Collection

# TransferRepresentation Implementations

## Topics

### Instance Properties

var body: Never

A builder expression that describes the process of importing and exporting an item.

### Instance Methods

func exportingCondition((Self.Item) -> Bool) -> _ConditionalTransferRepresentation&lt;Self>

Prevents the system from exporting an item if it does not meet the supplied condition.

func suggestedFileName((Self.Item) -> String?) -> some TransferRepresentation&lt;Self.Item> 

Provides a filename to use if the receiver chooses to write the item to disk.

func suggestedFileName(String) -> some TransferRepresentation&lt;Self.Item> 

Provides a filename to use if the receiver chooses to write the item to disk.

func visibility(TransferRepresentationVisibility) -> some TransferRepresentation&lt;Self.Item> 

Specifies the kinds of apps and processes that can see an item in transit.

### Type Aliases

typealias Body

The transfer representation for the item.

typealias Item

The type of the item that’s being transferred.

