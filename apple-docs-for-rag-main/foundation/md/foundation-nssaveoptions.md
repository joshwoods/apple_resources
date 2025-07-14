

- Foundation
-  NSSaveOptions 

Enumeration

# NSSaveOptions

The saveOptions method returns one of the following constants to indicate how to deal with saving any modified documents:

Mac Catalyst 13.0+macOS 10.0+

``` source
enum NSSaveOptions
```

## Topics

### Constants

case yes

Indicates a modified document should be saved on closing without asking the user.

case no

Indicates a modified document should not be saved on closing.

case ask

Indicates the user should be asked before saving any modified documents on closing. When no option is specified, this is the default.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

