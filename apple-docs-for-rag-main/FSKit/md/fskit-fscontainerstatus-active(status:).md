

- FSKit
- FSContainerStatus
-  active(status:) 

Type Method

# active(status:)

Returns a active container status instance with the provided error status.

macOS 15.4+

``` source
class func active(status errorStatus: any Error) -> Self
```

## Parameters 

`errorStatus`  

The error status, if any, for the new instance.

## See Also

### Creating a container status instance

class func blocked(status: any Error) -> Self

Returns a blocked container status instance with the provided error status.

class func notReady(status: any Error) -> Self

Returns a not-ready container status instance with the provided error status.

class func ready(status: any Error) -> Self

Returns a ready container status instance with the provided error status.

