

- Core Graphics
-  CGDataProviderDirectCallbacks 

Structure

# CGDataProviderDirectCallbacks

Defines pointers to client-defined callback functions that manage the sending of data for a direct-access data provider.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGDataProviderDirectCallbacks
```

## Overview

You supply a CGDataProviderDirectCallbacks structure to the function init(directInfo:size:callbacks:) to create a data provider for direct access. The functions specified by the CGDataProviderDirectCallbacks structure are responsible for copying data a block at a time to a memory buffer for Core Graphics to use. The functions are also responsible for handling the data provider’s basic memory management. For the callback to work, one of the `getBytePointer` and `getBytesAtPosition` parameters must be non-`NULL`. If both are non-`NULL`, then `getBytePointer` is used to access the data.

## Topics

### Initializers

init()

init(version: UInt32, getBytePointer: CGDataProviderGetBytePointerCallback?, releaseBytePointer: CGDataProviderReleaseBytePointerCallback?, getBytesAtPosition: CGDataProviderGetBytesAtPositionCallback?, releaseInfo: CGDataProviderReleaseInfoCallback?)

### Instance Properties

var getBytePointer: CGDataProviderGetBytePointerCallback?

A pointer to a function that returns a pointer to the provider’s data. For more information, see CGDataProviderGetBytePointerCallback.

var getBytesAtPosition: CGDataProviderGetBytesAtPositionCallback?

A pointer to a function that copies data from the provider.

var releaseBytePointer: CGDataProviderReleaseBytePointerCallback?

A pointer to a function that Core Graphics calls to release a pointer to the provider’s data. For more information, see CGDataProviderReleaseBytePointerCallback.

var releaseInfo: CGDataProviderReleaseInfoCallback?

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

var version: UInt32

The version of this structure. It should be set to 0.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating Direct-Access Data Providers

init?(directInfo: UnsafeMutableRawPointer?, size: off_t, callbacks: UnsafePointer&lt;CGDataProviderDirectCallbacks>)

Creates a direct-access data provider.

init?(data: CFData)

Creates a data provider that reads from a CFData object.

init?(url: CFURL)

Creates a direct-access data provider that uses a URL to supply data.

init?(dataInfo: UnsafeMutableRawPointer?, data: UnsafeRawPointer, size: Int, releaseData: CGDataProviderReleaseDataCallback)

Creates a direct-access data provider that uses data your program supplies.

init?(filename: UnsafePointer&lt;CChar>)

Creates a direct-access data provider that uses a file to supply data.

typealias CGDataProviderGetBytePointerCallback

A callback function that returns a generic pointer to the provider data.

typealias CGDataProviderGetBytesAtPositionCallback

A callback function that copies data from the provider into a Core Graphics buffer.

typealias CGDataProviderReleaseBytePointerCallback

A callback function that releases the pointer Core Graphics obtained by calling CGDataProviderGetBytePointerCallback.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

typealias CGDataProviderReleaseDataCallback

A callback function that releases data you supply to the function init(dataInfo:data:size:releaseData:).

