

- Foundation
- FileHandle
-  writeabilityHandler 

Instance Property

# writeabilityHandler

The block to use for writing the contents of the file handle asynchronously.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var writeabilityHandler: ((FileHandle) -> Void)? { get set }
```

## Discussion

The default value of this property is `nil`. Assigning a valid Block object to this property creates a dispatch source for writing the contents of the file or socket. Your block is submitted to the file handle’s dispatch queue when there is room available to write more data. When writing a file, your handler block is typically executed repeatedly until the entire contents of the file have been written. When writing data to a socket, your handler block is executed whenever the socket is ready to accept more data.

The block you provide must accept a single parameter that is the current file handle. The return type of your block should be `void`.

To stop writing data to the file or socket, set the value of this property to `nil`. Doing so cancels the dispatch source and cleans up the file handle’s structures appropriately.

## See Also

### Monitoring for Readability and Writability

var readabilityHandler: ((FileHandle) -> Void)?

The block to use for reading the contents of the file handle asynchronously.

