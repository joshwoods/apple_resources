

- Core Telephony
-  CTError 

Structure

# CTError

A type representing a Core Telephony error.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.10+

``` source
struct CTError
```

## Topics

### Getting Error Properties

var domain: Int32

A numeric indication of the error domain.

var error: Int32

A code indicating the specific error.

### Identifying Error Domains

Error Domains

Error domains used by Core Telephony errors.

### Initializers

init()

Creates a Core Telephony error instance.

init(domain: Int32, error: Int32)

Creates a Core Telephony error instance with the given values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

