

- OSLog
- OSLogMessageComponent
-  OSLogMessageComponent.Argument 

Enumeration

# OSLogMessageComponent.Argument

An object representing data that corresponds to an argument in a message payload.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Argument
```

## Topics

### Constants

case data(Data)

A data object returned by the OSLog API that corresponds to the argument.

case double(Double)

A double returned by the OSLog API that corresponds to the argument.

case signed(Int64)

A signed 64-bit integer returned by the OSLog API that corresponds to the argument.

case string(String)

A string returned by the OSLog API that corresponds to the argument.

case undefined

A undefined object returned by the OSLog API that corresponds to the argument.

case unsigned(UInt64)

An unsigned 64-bit integer returned by the OSLog API that corresponds to the argument.

## See Also

### Reading the Argument

var argument: OSLogMessageComponent.Argument

The argument passed into the message component.

var argumentCategory: OSLogMessageComponent.ArgumentCategory

The type of argument that corresponds to the placeholder.

enum ArgumentCategory

The data type corresponding to the argument provided in a message payload.

