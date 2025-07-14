

- Accelerate
-  BNNSGraphContextSetMessageLogMask(\_:\_:) 

Function

# BNNSGraphContextSetMessageLogMask(\_:\_:)

Sets mask for log messages that are logged (either via `os_log` or the user specified callback)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextSetMessageLogMask(
    _ context: bnns_graph_context_t,
    _ log_level_mask: UInt32
) -> Int32
```

## Discussion

- `context`: context to set callbacks for

- `log_level_mask`: bitmask of levels to log for (Default is BNNSGraphMessageLevelUnsupported \| BNNSGraphMessageLevelWarning \| BNNSGraphMessageLevelError)

## See Also

### Specifying a graph’s compile-time message callback

func BNNSGraphCompileOptionsSetMessageLogMask(bnns_graph_compile_options_t, UInt32)

Sets the mask for compile-time messages.

struct BNNSGraphMessageLevel

Constants that specify the mask for compile-time messages.

func BNNSGraphCompileOptionsSetMessageLogCallback(bnns_graph_compile_options_t, bnns_graph_compile_message_fn_t, UnsafeMutablePointer&lt;bnns_user_message_data_t>?)

Specifies a customized callback function that reports compile-time messages.

typealias bnns_graph_compile_message_fn_t

The graph compile-message logging callback function.

struct bnns_user_message_data_t

Additional user-defined logging argument for message-logging callbacks.

