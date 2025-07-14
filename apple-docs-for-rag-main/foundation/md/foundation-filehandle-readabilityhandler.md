

- Foundation
- FileHandle
-  readabilityHandler 

Instance Property

# readabilityHandler

The block to use for reading the contents of the file handle asynchronously.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var readabilityHandler: ((FileHandle) -> Void)? { get set }
```

## Discussion

The default value of this property is `nil`. Assigning a valid Block object to this property creates a dispatch source for reading the contents of the file or socket. Your block is submitted to the file handle’s dispatch queue when there is data to read. When reading a file, your handler block is typically executed repeatedly until the entire contents of the file have been read. When reading data from a socket, your handler block is executed whenever there is data on the socket waiting to be read.

The block you provide must accept a single parameter that is the current file handle. The return type of your block should be `void`.

To stop reading the file or socket, set the value of this property to `nil`. Doing so cancels the dispatch source and cleans up the file handle’s structures appropriately.

## See Also

### Monitoring for Readability and Writability

var writeabilityHandler: ((FileHandle) -> Void)?

The block to use for writing the contents of the file handle asynchronously.

