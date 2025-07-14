

- Foundation
- NSUserUnixTask
-  standardError 

Instance Property

# standardError

The standard error stream.

macOS 10.8+

``` source
var standardError: FileHandle? { get set }
```

## Discussion

Setting to `nil` will bind the stream to `/dev/null`.

The default is `nil`.

## See Also

### Standard Unix Streams

var standardInput: FileHandle?

The standard input stream.

var standardOutput: FileHandle?

The standard output stream.

