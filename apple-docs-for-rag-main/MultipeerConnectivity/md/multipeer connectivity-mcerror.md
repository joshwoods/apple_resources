

- Multipeer Connectivity
-  MCError 

Structure

# MCError

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
struct MCError
```

## Topics

### Initializers

init(Code, userInfo: [String : Any])

### Instance Properties

var code: Code

var errorCode: Int

var errorUserInfo: [String : Any]

var hashValue: Int

var userInfo: [String : Any]

### Type Properties

static var cancelled: MCError.Code

static var errorDomain: String

static var invalidParameter: MCError.Code

static var notConnected: MCError.Code

static var timedOut: MCError.Code

static var unavailable: MCError.Code

static var unknown: MCError.Code

static var unsupported: MCError.Code

### Instance Methods

func hash(into: inout Hasher)

### Operator Functions

static func == (MCError, MCError) -> Bool

### Enumerations

enum Code

Error codes found in MCErrorDomain error domain `NSError` objects returned by methods in the Multipeer Connectivity framework.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

