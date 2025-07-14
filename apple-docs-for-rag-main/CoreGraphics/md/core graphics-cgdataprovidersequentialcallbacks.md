

- Core Graphics
-  CGDataProviderSequentialCallbacks 

Structure

# CGDataProviderSequentialCallbacks

Defines a structure containing pointers to client-defined callback functions that manage the sending of data for a sequential-access data provider.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGDataProviderSequentialCallbacks
```

## Overview

The functions specified by the `CGDataProviderSequentialCallbacks` structure are responsible for sequentially copying data to a memory buffer for Core Graphics to use. The functions are also responsible for handling the data provider’s basic memory management. You supply a `CGDataProviderSequentialCallbacks` structure to the function init(sequentialInfo:callbacks:) to create a sequential-access data provider.

## Topics

### Initializers

init()

init(version: UInt32, getBytes: CGDataProviderGetBytesCallback?, skipForward: CGDataProviderSkipForwardCallback?, rewind: CGDataProviderRewindCallback?, releaseInfo: CGDataProviderReleaseInfoCallback?)

### Instance Properties

var getBytes: CGDataProviderGetBytesCallback?

A pointer to a function that copies data from the provider. For more information, see CGDataProviderGetBytesCallback.

var releaseInfo: CGDataProviderReleaseInfoCallback?

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

var rewind: CGDataProviderRewindCallback?

A pointer to a function Core Graphics calls to return the provider to the beginning of the data stream. For more information, see CGDataProviderRewindCallback.

var skipForward: CGDataProviderSkipForwardCallback?

A pointer to a function that Core Graphics calls to advance the stream of data supplied by the provider.

var version: UInt32

The version of this structure. It should be set to 0.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating Sequential-Access Data Providers

init?(sequentialInfo: UnsafeMutableRawPointer?, callbacks: UnsafePointer&lt;CGDataProviderSequentialCallbacks>)

Creates a sequential-access data provider.

typealias CGDataProviderRewindCallback

A callback function that moves the current position in the data stream back to the beginning.

typealias CGDataProviderGetBytesCallback

A callback function that copies from a provider data stream into a Core Graphics buffer.

typealias CGDataProviderSkipForwardCallback

A callback function that advances the current position in the data stream supplied by the provider.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

