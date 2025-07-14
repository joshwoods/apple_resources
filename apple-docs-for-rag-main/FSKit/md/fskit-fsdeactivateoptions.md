

- FSKit
-  FSDeactivateOptions 

Structure

# FSDeactivateOptions

Options that affect the behavior of deactivate methods.

macOS 15.4+

``` source
struct FSDeactivateOptions
```

## Topics

### Deactivation options

static var force: FSDeactivateOptions

An option to force deactivation.

### Working with raw values

init(rawValue: Int)

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

### Handling activation and deactivation

func activate(options: FSTaskOptions, replyHandler: (FSItem?, (any Error)?) -> Void)

Activates the volume using the specified options.

**Required**

class FSItem

A distinct object in a file hierarchy, such as a file, directory, symlink, socket, and more.

func deactivate(options: FSDeactivateOptions, replyHandler: ((any Error)?) -> Void)

Tears down a previously initialized volume instance.

**Required**

