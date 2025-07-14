

- Foundation
- InputStream
-  init(URL:) 

Initializer

# init(URL:)

Creates and returns an initialized `NSInputStream` object that reads data from the file at a given URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(URL url: URL)
```

## Parameters 

`url`  

The URL to the file.

## Return Value

An initialized `NSInputStream` object that reads data from the URL at `url`.

## Discussion

The stream must be opened before it can be used.

## See Also

### Creating Streams

init(data: Data)

Initializes and returns an `NSInputStream` object for reading from a given `NSData` object.

convenience init?(fileAtPath: String)

Initializes and returns an `NSInputStream` object that reads data from the file at a given path.

init?(url: URL)

Initializes and returns an `NSInputStream` object that reads data from the file at a given URL.

