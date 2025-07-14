

- Accelerate
-  bnns_user_message_data_t 

Structure

# bnns_user_message_data_t

Additional user-defined logging argument for message-logging callbacks.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct bnns_user_message_data_t
```

## Topics

### Initializers

init()

init(size: Int, data: UnsafeMutableRawPointer?)

Creates a logging argument structure from the pointer to the additional logging data.

### Instance Properties

var data: UnsafeMutableRawPointer?

A pointer to the additional logging data.

var size: Int

The size of the additional logging data.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Specifying a graph’s compile-time message callback

func BNNSGraphCompileOptionsSetMessageLogMask(bnns_graph_compile_options_t, UInt32)

Sets the mask for compile-time messages.

func BNNSGraphContextSetMessageLogMask(bnns_graph_context_t, UInt32) -> Int32

Sets mask for log messages that are logged (either via `os_log` or the user specified callback)

struct BNNSGraphMessageLevel

Constants that specify the mask for compile-time messages.

func BNNSGraphCompileOptionsSetMessageLogCallback(bnns_graph_compile_options_t, bnns_graph_compile_message_fn_t, UnsafeMutablePointer&lt;bnns_user_message_data_t>?)

Specifies a customized callback function that reports compile-time messages.

typealias bnns_graph_compile_message_fn_t

The graph compile-message logging callback function.

