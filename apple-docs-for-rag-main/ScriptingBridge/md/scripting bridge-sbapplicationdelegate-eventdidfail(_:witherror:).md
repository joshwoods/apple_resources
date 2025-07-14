

- Scripting Bridge
- SBApplicationDelegate
-  eventDidFail(\_:withError:) 

Instance Method

# eventDidFail(\_:withError:)

Sent by an `SBApplication` object when a target application returns an error Apple event.

Mac Catalyst 13.0+macOS 10.5+

``` source
func eventDidFail(
    _ event: UnsafePointer,
    withError error: any Error
) -> Any?
```

**Required**

## Parameters 

`event`  

A pointer to the Apple event sent to the target application causing the error.

`error`  

An object containing information about the error Apple event. Specific information may be included in the `useInfo` dictionary of the error object. The following table shows the possible keys for this dictionary.

| Key | Description |
|----|----|
| ErrorBriefMessage | A short human-readable description of the error, as an NSString |
| ErrorExpectedType | The type of data the target application expected, as an NSAppleEventDescriptor object. |
| ErrorOffendingObject | The object that caused the error. |
| ErrorString | A full human-readable description of the error, as an NSString object. |
| ErrorNumber | The Apple event error number, as an NSNumber object. |

## Return Value

If you return a result, it will become the result of the sendEvent(_:) that failed. Can be `nil`.

