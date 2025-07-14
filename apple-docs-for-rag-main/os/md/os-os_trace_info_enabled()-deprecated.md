

- os
-  os_trace_info_enabled() Deprecated

Function

# os_trace_info_enabled()

Returns whether info level trace information is enabled.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.13DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
func os_trace_info_enabled() -> Bool
```

Deprecated

Use os_log_info_enabled instead.

## Discussion

Generally, trace points should not involve expensive operations, however some circumstances warrant it. Use this function to do expensive work only when info level trace messages are enabled.

## See Also

### Deprecated Functions

func os_trace_debug_enabled() -> Bool

Returns whether debug level trace information is enabled.

Deprecated

func os_trace_type_enabled(UInt8) -> Bool

Returns whether the specified info level trace information is enabled.

Deprecated

