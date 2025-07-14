

- Quartz
-  IKImageBrowserCellState 

Structure

# IKImageBrowserCellState

The possible states for the browser cell. These values are used by the cellState() method.

macOS 10.4+

``` source
struct IKImageBrowserCellState
```

## Topics

### Constants

var IKImageStateNoImage: IKImageBrowserCellState

Returned until a thumbnail has been created from the represented object.

var IKImageStateInvalid: IKImageBrowserCellState

The thumbnail is invalid. For example, an unsupported image is provided.

var IKImageStateReady: IKImageBrowserCellState

The receiver’s represented object has been set and the cell is ready to display.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Informal Protocols

struct IKImageBrowserDropOperation

These constants specify the locations for dropping items onto the browser view. Used by the method setDrop(_:dropOperation:).

