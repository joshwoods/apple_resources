

- os
-  os_trace_type_enabled(\_:) Deprecated

Function

# os_trace_type_enabled(\_:)

Returns whether the specified info level trace information is enabled.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.13DeprecatedtvOS 8.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
func os_trace_type_enabled(_ type: UInt8) -> Bool
```

Deprecated

Use isEnabled(type:) instead.

## Parameters 

`type`  

The type of trace to check. Possible values are OS_TRACE_TYPE_DEBUG and OS_TRACE_TYPE_INFO.

## Discussion

Generally, trace points should not involve expensive operations, however some circumstances warrant it. Use this function to do expensive work only when a given level of trace messages are enabled.

## See Also

### Deprecated Functions

func os_trace_debug_enabled() -> Bool

Returns whether debug level trace information is enabled.

Deprecated

func os_trace_info_enabled() -> Bool

Returns whether info level trace information is enabled.

Deprecated

