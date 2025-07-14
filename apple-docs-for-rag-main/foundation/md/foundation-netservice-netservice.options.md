

- Foundation
- NetService
-  NetService.Options 

Structure

# NetService.Options

These constants specify options for a network service.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
struct Options
```

## Topics

### Constants

static var noAutoRename: NetService.Options

Specifies that the network service should not rename itself in the event of a name collision.

static var listenForConnections: NetService.Options

static var noAutoRename: NetService.Options

Specifies that the network service should not rename itself in the event of a name collision.

static var listenForConnections: NetService.Options

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

NSNetServices Errors

If an error occurs, the delegate error-handling methods return a dictionary with the following keys.

enum ErrorCode

These constants identify errors that can occur when accessing net services.

