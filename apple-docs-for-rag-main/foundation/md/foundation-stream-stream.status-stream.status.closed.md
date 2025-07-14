

- Foundation
- Stream
- Stream.Status
-  Stream.Status.closed 

Case

# Stream.Status.closed

The stream is closed (close() has been called on it).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case closed
```

## See Also

### Enumeration Cases

case atEnd

There is no more data to read, or no more data can be written to the stream. When this status is returned, the stream is in a “non-blocking” mode and no data are available.

case error

The remote end of the connection can’t be contacted, or the connection has been severed for some other reason.

case notOpen

The stream is not open for reading or writing. This status is returned before the underlying call to open a stream but after it’s been created.

case open

The stream is open, but no reading or writing is occurring.

case opening

The stream is in the process of being opened for reading or for writing. For network streams, this status might include the time after the stream was opened, but while network DNS resolution is happening.

case reading

Data is being read from the stream. This status would be returned if code on another thread were to call streamStatus on the stream while a read(_:maxLength:) call (InputStream) was in progress.

case writing

Data is being written to the stream. This status would be returned if code on another thread were to call streamStatus on the stream while a write(_:maxLength:) call (OutputStream) was in progress.

case atEnd

There is no more data to read, or no more data can be written to the stream. When this status is returned, the stream is in a “non-blocking” mode and no data are available.

case error

The remote end of the connection can’t be contacted, or the connection has been severed for some other reason.

case notOpen

The stream is not open for reading or writing. This status is returned before the underlying call to open a stream but after it’s been created.

case open

The stream is open, but no reading or writing is occurring.

case opening

The stream is in the process of being opened for reading or for writing. For network streams, this status might include the time after the stream was opened, but while network DNS resolution is happening.

case reading

Data is being read from the stream. This status would be returned if code on another thread were to call streamStatus on the stream while a read(_:maxLength:) call (InputStream) was in progress.

case writing

Data is being written to the stream. This status would be returned if code on another thread were to call streamStatus on the stream while a write(_:maxLength:) call (OutputStream) was in progress.

