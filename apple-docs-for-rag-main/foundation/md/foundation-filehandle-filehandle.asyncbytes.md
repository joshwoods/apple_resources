

- Foundation
- FileHandle
-  FileHandle.AsyncBytes 

Structure

# FileHandle.AsyncBytes

An asynchronous sequence of bytes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AsyncBytes
```

## Overview

Use the `for`-`await`-`in` syntax to iterate over the bytes in this sequence. For text files, you can also use its `characters`, `unicodeScalars`, or `lines` properties to retrieve the contents in a more convenient format. Since all of these properties conform to AsyncSequence, as does the FileHandle property bytes, you can use methods defined by AsyncSequence to perform powerful inline processing. For example, you can skip the first `n` bytes of the file with `myFileHandle.bytes.prefix(n)`.

## Topics

### Adapting Textual Sequences

struct AsyncCharacterSequence

An asynchronous sequence of characters.

struct AsyncUnicodeScalarSequence

An asychronous sequence of Unicode scalar values.

struct AsyncLineSequence

An asynchronous sequence of lines of text.

### Structures

struct Iterator

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Reading from a File Handle Asynchronously

var bytes: FileHandle.AsyncBytes

The file’s contents, as an asynchronous sequence of bytes.

