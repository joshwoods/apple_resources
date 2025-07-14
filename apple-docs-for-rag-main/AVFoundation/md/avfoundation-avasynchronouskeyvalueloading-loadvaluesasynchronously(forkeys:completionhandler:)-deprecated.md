

- AVFoundation
- AVAsynchronousKeyValueLoading
-  loadValuesAsynchronously(forKeys:completionHandler:) Deprecated

Instance Method

# loadValuesAsynchronously(forKeys:completionHandler:)

Tells the asset to load the values of all of the specified keys that aren’t already loaded.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func loadValuesAsynchronously(
    forKeys keys: [String],
    completionHandler handler: (() -> Void)? = nil
)
```

``` source
func loadValues(forKeys keys: [String]) async
```

**Required**

Deprecated

Use load(_:) instead.

## Parameters 

`keys`  

An array of strings containing the keys to load. The keys are the property names of a class that adopts the protocol.

`handler`  

The closure the system calls when the load request completes.

## Mentioned in 

Loading media data asynchronously

## Discussion

Regardless of the number of keys specified, the system calls the completion handler only once per invocation of this method. The system calls this method:

- Synchronously if the asset already loaded the specified keys, or if an I/O error or other format-related error occurs immediately.

- Asynchronously when the values of the specified keys become loaded, if a loading error occurs at a later stage of processing, or you cancel loading. The system calls the closure on a background queue, so you should dispatch control back to the main queue before performing any user interface-related operations.

The completion states of the specified keys aren’t necessarily the same—some may return loaded, and others may have failed. Check the status of each key individually using the statusOfValue(forKey:error:) method.

The following example shows how to use this method to load an asset’s isPlayable key:

```
// Load the asset's "commonMetadata" key
[asset loadValuesAsynchronouslyForKeys:@[@"commonMetadata"] completionHandler:^{
    NSError *error = nil;
    AVKeyValueStatus status =
        [asset statusOfValueForKey:@"commonMetadata" error:&error];
    switch (status) {
        case AVKeyValueStatusLoaded:
            // The property successfully loaded. Continue processing.
             break;
        case AVKeyValueStatusFailed:
            // Examine the NSError pointer to determine the failure.
            break;
        case AVKeyValueStatusCancelled:
            // The asset canceled loading.
            break;
        default:
            // Handle all other cases.
            break;
    }
}];
```

## See Also

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

func statusOfValue(forKey: String, error: NSErrorPointer) -> AVKeyValueStatus

Returns a status that indicates whether a property value is immediately available without blocking the calling thread.

**Required**

Deprecated

enum AVKeyValueStatus

Values that indicate the loaded status of a property.

Deprecated

