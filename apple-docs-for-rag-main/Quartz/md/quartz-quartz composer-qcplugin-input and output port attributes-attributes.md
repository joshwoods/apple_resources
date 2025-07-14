

- Quartz
- Quartz Composer
- QCPlugIn
-  Input and Output Port Attributes 

API Collection

# Input and Output Port Attributes

Attributes for input and output ports.

## Topics

### Constants

let QCPortAttributeTypeKey: String

The key for the port type. The associated value can be of any of the following constants: QCPortTypeBoolean, QCPortTypeIndex, QCPortTypeNumber, QCPortTypeString, QCPortTypeColor, QCPortTypeImage, or QCPortTypeStructure.

Deprecated

let QCPortAttributeNameKey: String

The key for the port name.

Deprecated

let QCPortAttributeMinimumValueKey: String

The key for the port minimum value.

Deprecated

let QCPortAttributeMaximumValueKey: String

The key for the port maximum value.

Deprecated

let QCPortAttributeDefaultValueKey: String

The key for the port default value. You can use this key only for value ports (Boolean, Index, Number, Color and String).

Deprecated

let QCPortAttributeMenuItemsKey: String

The key for the menu items.

Deprecated

## See Also

### Constants

Patch Attributes

Attributes for custom patches.

Port Input and Output Types

Data types for input and output ports.

Pixel Formats

Supported image pixel formats.

Execution Arguments

Arguments to the method execute(_:atTime:withArguments:).

struct QCPlugInExecutionMode

Execution modes for custom patches.

Deprecated

struct QCPlugInTimeMode

Time modes for custom patches.

Deprecated

