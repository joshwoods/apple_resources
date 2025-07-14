

- AVFoundation
-  AVAsynchronousKeyValueLoading 

Protocol

# AVAsynchronousKeyValueLoading

A protocol that defines the interface to load media data asynchronously.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVAsynchronousKeyValueLoading
```

## Mentioned in 

Loading media data asynchronously

## Overview

Loading media data takes an amount of time that depends on factors including the media’s size, location, device capabilities, network conditions, and so on. To optimize performance, AVAsset defers loading its media data until you query its properties or perform an operation that requires it. This means that performing these actions from a synchronous context would block the calling thread for an unknown amount of time, which would result in a poor user experience, and may even cause your app to crash. For this reason, you must load media data asynchronously.

Call the asynchronous load(_:) method to retrieve the values of media properties, or determine the loaded status of a property by calling the status(of:) method. See Loading media data asynchronously for more information.

## Topics

### Loading Property Values

func load&lt;T>(AVAsyncProperty&lt;Self, T>) async throws -> T

Loads a property asynchronously and returns the value.

func load&lt;A, B>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>) async throws -> (A, B)

Loads two properties asynchronously and returns the values.

func load&lt;A, B, C>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>) async throws -> (A, B, C)

Loads three properties asynchronously and returns the values.

func load&lt;A, B, C, D>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>) async throws -> (A, B, C, D)

Loads four properties asynchronously and returns the values.

func load&lt;A, B, C, D, E>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>) async throws -> (A, B, C, D, E)

Loads five properties asynchronously and returns the values.

func load&lt;A, B, C, D, E, F>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>, AVAsyncProperty&lt;Self, F>) async throws -> (A, B, C, D, E, F)

Loads six properties asynchronously and returns the values.

func load&lt;A, B, C, D, E, F, G>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>, AVAsyncProperty&lt;Self, F>, AVAsyncProperty&lt;Self, G>) async throws -> (A, B, C, D, E, F, G)

Loads seven properties asynchronously and returns the values.

func load&lt;A, B, C, D, E, F, G, H>(AVAsyncProperty&lt;Self, A>, AVAsyncProperty&lt;Self, B>, AVAsyncProperty&lt;Self, C>, AVAsyncProperty&lt;Self, D>, AVAsyncProperty&lt;Self, E>, AVAsyncProperty&lt;Self, F>, AVAsyncProperty&lt;Self, G>, AVAsyncProperty&lt;Self, H>) async throws -> (A, B, C, D, E, F, G, H)

Loads eight properties asynchronously and returns the values.

### Determining the Loaded Status

func status&lt;T>(of: AVAsyncProperty&lt;Self, T>) -> AVAsyncProperty&lt;Self, T>.Status

Returns a value that indicates the loaded status of a property.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

func loadValuesAsynchronously(forKeys: [String], completionHandler: (() -> Void)?)

Tells the asset to load the values of all of the specified keys that aren’t already loaded.

**Required**

Deprecated

func statusOfValue(forKey: String, error: NSErrorPointer) -> AVKeyValueStatus

Returns a status that indicates whether a property value is immediately available without blocking the calling thread.

**Required**

Deprecated

enum AVKeyValueStatus

Values that indicate the loaded status of a property.

Deprecated

## Relationships

### Conforming Types

- AVAsset
- AVAssetTrack
- AVComposition
- AVCompositionTrack
- AVFragmentedAsset
- AVFragmentedAssetTrack
- AVFragmentedMovie
- AVFragmentedMovieTrack
- AVMetadataItem
- AVMovie
- AVMovieTrack
- AVMutableComposition
- AVMutableCompositionTrack
- AVMutableMetadataItem
- AVMutableMovie
- AVMutableMovieTrack
- AVURLAsset

## See Also

### Property loading

class AVAsyncProperty

An asynchronous property that constrains its type and value.

class AVPartialAsyncProperty

An asynchronous property that constrains its type.

class AVAnyAsyncProperty

A base class for asynchronous properties.

