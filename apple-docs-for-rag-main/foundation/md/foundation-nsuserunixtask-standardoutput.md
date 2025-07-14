

- Foundation
- NSUserUnixTask
-  standardOutput 

Instance Property

# standardOutput

The standard output stream.

macOS 10.8+

``` source
var standardOutput: FileHandle? { get set }
```

## Discussion

Setting to `nil` will bind the stream to `/dev/null`.

The default is `nil`.

## See Also

### Standard Unix Streams

var standardError: FileHandle?

The standard error stream.

var standardInput: FileHandle?

The standard input stream.

