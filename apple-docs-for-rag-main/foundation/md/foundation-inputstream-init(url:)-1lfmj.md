

- Foundation
- InputStream
-  init(url:) 

Initializer

# init(url:)

Initializes and returns an `NSInputStream` object that reads data from the file at a given URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(url: URL)
```

## Parameters 

`url`  

The URL to the file.

## Return Value

An initialized `NSInputStream` object that reads data from the file at `url`.

## Discussion

The stream must be opened before it can be used.

## See Also

### Creating Streams

convenience init?(URL: URL)

Creates and returns an initialized `NSInputStream` object that reads data from the file at a given URL.

init(data: Data)

Initializes and returns an `NSInputStream` object for reading from a given `NSData` object.

convenience init?(fileAtPath: String)

Initializes and returns an `NSInputStream` object that reads data from the file at a given path.

