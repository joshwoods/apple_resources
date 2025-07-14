

- Foundation
- InputStream
-  init(data:) 

Initializer

# init(data:)

Initializes and returns an `NSInputStream` object for reading from a given `NSData` object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(data: Data)
```

## Parameters 

`data`  

The data object from which to read. The contents of `data` are copied.

## Return Value

An initialized `NSInputStream` object for reading from `data`.

## Discussion

The stream must be opened before it can be used.

## See Also

### Creating Streams

convenience init?(URL: URL)

Creates and returns an initialized `NSInputStream` object that reads data from the file at a given URL.

convenience init?(fileAtPath: String)

Initializes and returns an `NSInputStream` object that reads data from the file at a given path.

init?(url: URL)

Initializes and returns an `NSInputStream` object that reads data from the file at a given URL.

