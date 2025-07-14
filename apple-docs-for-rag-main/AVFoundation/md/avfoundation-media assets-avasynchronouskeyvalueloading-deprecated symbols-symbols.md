

- AVFoundation
- Media assets
- AVAsynchronousKeyValueLoading
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Overview

See Loading media data asynchronously for information on the replacement API that’s based on Swift’s concurrency features.

## Topics

### Loading Property Values

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

## See Also

### Deprecated

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

