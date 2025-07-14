

- AVFoundation
- AVAsynchronousKeyValueLoading
-  statusOfValue(forKey:error:) Deprecated

Instance Method

# statusOfValue(forKey:error:)

Returns a status that indicates whether a property value is immediately available without blocking the calling thread.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func statusOfValue(
    forKey key: String,
    error outError: NSErrorPointer
) -> AVKeyValueStatus
```

**Required**

Deprecated

Use status(of:) instead.

## Parameters 

`key`  

The property whose status you want.

`outError`  

If the status of the value for the `key` is AVKeyValueStatus.failed, the system sets this pointer to an NSError object that describes the failure.

## Return Value

The current status of the requested key.

## See Also

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

func loadValuesAsynchronously(forKeys: [String], completionHandler: (() -> Void)?)

Tells the asset to load the values of all of the specified keys that aren’t already loaded.

**Required**

Deprecated

enum AVKeyValueStatus

Values that indicate the loaded status of a property.

Deprecated

