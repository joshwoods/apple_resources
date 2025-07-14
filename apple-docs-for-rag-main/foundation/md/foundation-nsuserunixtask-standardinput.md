

- Foundation
- NSUserUnixTask
-  standardInput 

Instance Property

# standardInput

The standard input stream.

macOS 10.8+

``` source
var standardInput: FileHandle? { get set }
```

## Discussion

Setting to `nil` will bind the stream to `/dev/null`.

The default is `nil`.

## See Also

### Standard Unix Streams

var standardError: FileHandle?

The standard error stream.

var standardOutput: FileHandle?

The standard output stream.

