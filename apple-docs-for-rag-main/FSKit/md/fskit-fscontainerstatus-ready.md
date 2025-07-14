

- FSKit
- FSContainerStatus
-  ready 

Type Property

# ready

A status that represents a ready container with no error.

macOS 15.4+

``` source
class var ready: FSContainerStatus { get }
```

## Discussion

This value is a FSContainerStatus with a state that is ready, and a status that is `nil`.

## See Also

### Using common status values

class var active: FSContainerStatus

A status that represents an active container with no error.

