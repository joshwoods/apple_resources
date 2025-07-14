

- os
-  Logger 

Structure

# Logger

An object for writing interpolated string messages to the unified logging system.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct Logger
```

## Mentioned in 

Generating Log Messages from Your Code

## Overview

Create a Logger structure and use it to log messages about your app’s behavior. When logging a message, you specify the message and any program variables or custom data to help you assess the state of your app. You also choose a log level to indicate the severity of that message. The system records log messages in memory and, in some cases, also writes those messages to an on-disk data store. The log level determines which messages stay in memory and which go to disk.

When you create a Logger structure, assign an optional subsystem and category string to add context to all messages you log. A subsystem corresponds to a large functional area of your app, and a category corresponds to a specific area within a particular subsystem. When diagnosing problems, use those strings to filter out unrelated messages.

To log a message, call the method that represents the appropriate log level for that message. To create the message, use a Swift string. Strings may contain interpolated values, such as signed and unsigned integers, floating-point and double values, Booleans, other strings, Objective-C objects, and types that conform to the CustomStringConvertible protocol. You can also include metatypes such as `Int.self`.

```
let logger = Logger()
let x = 42
logger.info("The answer is \(x)")
```

When you include an interpolated string or custom object in your message, the system redacts the value of that string or object by default. This behavior prevents the system from leaking potentially user-sensitive information in the log files, such as the user’s account information. If the data doesn’t contain sensitive information, change the privacy option of that value when logging the information. In the following code example, the system redacts the account information in the first log message, but displays the user’s selection in the second log message:

```
logger.log("Paid with bank account \(accountNumber)")   // Redacted!
logger.log("Ordered smoothie \(smoothieName, privacy: .public)")  // Visible
```

## Topics

### Creating a Logger

init()

Creates a logger that writes to the default subsystem.

init(subsystem: String, category: String)

Creates a logger using the specified subsystem and category.

init(OSLog)

Creates a logger that writes to the specified log.

class OSLog

A container of related log messages.

### Logging a Message

func log(OSLogMessage)

Writes a message to the log using the default log type.

func log(level: OSLogType, OSLogMessage)

Writes a message to the log using the specified log type.

struct OSLogType

The various log levels that the unified logging system provides.

struct OSLogMessage

An object that represents a log message.

### Logging a Scoped Message

func notice(OSLogMessage)

Writes a message to the log using the default log type.

func debug(OSLogMessage)

Writes a debug message to the log.

func trace(OSLogMessage)

Writes a trace message to the log.

func info(OSLogMessage)

Writes an informative message to the log.

func error(OSLogMessage)

Writes information about an error to the log.

func warning(OSLogMessage)

Writes information about a warning to the log.

func fault(OSLogMessage)

Writes a message to the log about a bug that occurs when your app executes.

func critical(OSLogMessage)

Writes a message to the log about a critical event in your app’s execution.

## Relationships

### Conforms To

- Sendable

## See Also

### Log Messages

Message Argument Formatters

Manage the privacy and presentation of the message’s interpolated values using type-aware formatters.

struct OSLogType

The various log levels that the unified logging system provides.

