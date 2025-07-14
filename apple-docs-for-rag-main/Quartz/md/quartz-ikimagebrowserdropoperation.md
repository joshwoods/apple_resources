

- Quartz
-  IKImageBrowserDropOperation 

Structure

# IKImageBrowserDropOperation

These constants specify the locations for dropping items onto the browser view. Used by the method setDrop(_:dropOperation:).

macOS 10.4+

``` source
struct IKImageBrowserDropOperation
```

## Topics

### Constants

var IKImageBrowserDropOn: IKImageBrowserDropOperation

Drop the item on the cell.

var IKImageBrowserDropBefore: IKImageBrowserDropOperation

Drop the item before the cell.

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

struct IKImageBrowserCellState

The possible states for the browser cell. These values are used by the cellState() method.

