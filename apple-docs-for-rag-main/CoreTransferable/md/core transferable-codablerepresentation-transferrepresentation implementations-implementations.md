

- Core Transferable
- CodableRepresentation
-  TransferRepresentation Implementations 

API Collection

# TransferRepresentation Implementations

## Topics

### Instance Methods

func exportingCondition((Self.Item) -> Bool) -> _ConditionalTransferRepresentation&lt;Self>

Prevents the system from exporting an item if it does not meet the supplied condition.

func suggestedFileName((Self.Item) -> String?) -> some TransferRepresentation&lt;Self.Item> 

Provides a filename to use if the receiver chooses to write the item to disk.

func suggestedFileName(String) -> some TransferRepresentation&lt;Self.Item> 

Provides a filename to use if the receiver chooses to write the item to disk.

func visibility(TransferRepresentationVisibility) -> some TransferRepresentation&lt;Self.Item> 

Specifies the kinds of apps and processes that can see an item in transit.

