

- IOUSBHost
-  IOUSBHostAbortOption 

Enumeration

# IOUSBHostAbortOption

Options for aborting pending input/output requests.

Mac Catalyst 14.0+macOS 10.15+

``` source
enum IOUSBHostAbortOption
```

## Topics

### Options

case synchronous

The option to abort input/output requests synchronously.

case asynchronous

The option to abort input/output requests asynchronously.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

