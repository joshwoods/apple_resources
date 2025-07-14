

- Apple Archive
- ArchiveStream
-  process(readingFrom:writingTo:selectUsing:flags:threadCount:) 

Type Method

# process(readingFrom:writingTo:selectUsing:flags:threadCount:)

Processes archive elements between two archive streams.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func process(
    readingFrom input: ArchiveStream,
    writingTo output: ArchiveStream,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) throws -> Int
```

## Parameters 

`input`  

The input stream.

`output`  

The output stream.

`filter`  

A closure that’s called for each entry that’s received by the stream.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

The number of processed bytes.

