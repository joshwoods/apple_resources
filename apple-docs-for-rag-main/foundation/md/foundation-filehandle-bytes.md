

- Foundation
- FileHandle
-  bytes 

Instance Property

# bytes

The file’s contents, as an asynchronous sequence of bytes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var bytes: FileHandle.AsyncBytes { get }
```

## Discussion

Use the `for`-`await`-`in` syntax to iterate over the bytes in this sequence. For text files, you can also use its `FileHandle/AsyncBytes/characters`, `FileHandle/AsyncBytes/unicodeScalars`, or `FileHandle/AsyncBytes/lines` properties to retrieve the contents in a more convenient format. Since all of these properties conform to AsyncSequence, as does bytes itself, you can use methods defined by AsyncSequence to perform powerful inline processing. For example, you can skip the first `n` bytes of the file with `myFileHandle.bytes.prefix(n)`.

Tip

Rather than creating a FileHandle to read a file asynchronously, you can instead use a `file://` URL in combination with the resourceBytes property in URL.

## See Also

### Reading from a File Handle Asynchronously

struct AsyncBytes

An asynchronous sequence of bytes.

