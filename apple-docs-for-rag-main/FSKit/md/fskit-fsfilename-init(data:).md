

- FSKit
- FSFileName
-  init(data:) 

Initializer

# init(data:)

Creates a filename by copying a character sequence data object.

macOS 15.4+

``` source
convenience init(data name: Data)
```

## Parameters 

`name`  

The data object containing the character sequence to use for the filename. The sequence terminates if a `NUL` character exists prior to `name.length`.

## Discussion

This initializer copies up to `name.length` characters of the sequence pointed to by `bytes`.

## See Also

### Creating a filename

convenience init(bytes: UnsafeBufferPointer&lt;CChar>)

convenience init(cString: UnsafeBufferPointer&lt;CChar>)

convenience init(string: String)

Creates a filename by copying a character sequence from a string instance.

