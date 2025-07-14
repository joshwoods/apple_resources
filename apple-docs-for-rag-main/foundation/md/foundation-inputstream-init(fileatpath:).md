

- Foundation
- InputStream
-  init(fileAtPath:) 

Initializer

# init(fileAtPath:)

Initializes and returns an `NSInputStream` object that reads data from the file at a given path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(fileAtPath path: String)
```

## Parameters 

`path`  

The path to the file.

## Return Value

An initialized `NSInputStream` object that reads data from the file at `path`.

## Discussion

The stream must be opened before it can be used.

## See Also

### Related Documentation

convenience init?(URL: URL)

Creates and returns an initialized `NSInputStream` object that reads data from the file at a given URL.

### Creating Streams

convenience init?(URL: URL)

Creates and returns an initialized `NSInputStream` object that reads data from the file at a given URL.

init(data: Data)

Initializes and returns an `NSInputStream` object for reading from a given `NSData` object.

init?(url: URL)

Initializes and returns an `NSInputStream` object that reads data from the file at a given URL.

