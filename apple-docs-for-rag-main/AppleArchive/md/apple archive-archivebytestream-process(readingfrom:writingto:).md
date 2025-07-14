

- Apple Archive
- ArchiveByteStream
-  process(readingFrom:writingTo:) 

Type Method

# process(readingFrom:writingTo:)

Processes data between two byte streams.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func process(
    readingFrom input: ArchiveByteStream,
    writingTo output: ArchiveByteStream
) throws -> Int64
```

## Parameters 

`input`  

The input stream.

`output`  

The output stream.

## Return Value

The number of processed bytes.

## Discussion

This function reads data from `input` and writes it to `output` until it reaches end-of-file (EOF).

