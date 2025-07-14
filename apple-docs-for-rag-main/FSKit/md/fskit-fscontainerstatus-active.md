

- FSKit
- FSContainerStatus
-  active 

Type Property

# active

A status that represents an active container with no error.

macOS 15.4+

``` source
class var active: FSContainerStatus { get }
```

## Discussion

This value is a FSContainerStatus with a state that is active, and has a status that is `nil`.

## See Also

### Using common status values

class var ready: FSContainerStatus

A status that represents a ready container with no error.

