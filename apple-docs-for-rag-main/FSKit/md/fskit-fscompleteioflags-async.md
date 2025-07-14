

- FSKit
- FSCompleteIOFlags
-  async 

Type Property

# async

A flag that requests that the file system module flush metadata I/O asynchronously.

macOS 15.4+

``` source
static var async: FSCompleteIOFlags { get }
```

## See Also

### Declaring I/O completion behaviors

static var read: FSCompleteIOFlags

A flag that describes a read operation.

static var write: FSCompleteIOFlags

A flag that describes a write operation.

