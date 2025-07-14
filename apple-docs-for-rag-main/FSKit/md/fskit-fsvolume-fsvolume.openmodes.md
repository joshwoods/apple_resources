

- FSKit
- FSVolume
-  FSVolume.OpenModes 

Structure

# FSVolume.OpenModes

Defined modes for opening a file.

macOS 15.4+

``` source
struct OpenModes
```

## Topics

### Declaring open modes

static var read: FSVolume.OpenModes

The read mode.

static var write: FSVolume.OpenModes

The write mode.

### Working with raw values

init(rawValue: UInt)

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

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

### Opening and closing

func openItem(FSItem, modes: FSVolume.OpenModes, replyHandler: ((any Error)?) -> Void)

Opens a file for access.

**Required**

func closeItem(FSItem, modes: FSVolume.OpenModes, replyHandler: ((any Error)?) -> Void)

Closes a file from further access.

**Required**

