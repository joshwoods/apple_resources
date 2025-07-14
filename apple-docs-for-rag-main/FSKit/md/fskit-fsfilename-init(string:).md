

- FSKit
- FSFileName
-  init(string:) 

Initializer

# init(string:)

Creates a filename by copying a character sequence from a string instance.

macOS 15.4+

``` source
convenience init(string name: String)
```

## Parameters 

`name`  

The string containing the character sequence to use for the filename.

## Discussion

This initializer copies the UTF-8 representation of the characters in `string`. If `string` contains a `NUL` character, the sequence terminates.

## See Also

### Creating a filename

convenience init(bytes: UnsafeBufferPointer&lt;CChar>)

convenience init(cString: UnsafeBufferPointer&lt;CChar>)

convenience init(data: Data)

Creates a filename by copying a character sequence data object.

