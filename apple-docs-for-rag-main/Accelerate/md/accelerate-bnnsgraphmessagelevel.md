

- Accelerate
-  BNNSGraphMessageLevel 

Structure

# BNNSGraphMessageLevel

Constants that specify the mask for compile-time messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSGraphMessageLevel
```

## Topics

### Graph message levels

init(UInt32)

Creates a new instance.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

### Instance properties

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSGraphMessageLevelInfo: BNNSGraphMessageLevel

A constant that specifies information message types.

var BNNSGraphMessageLevelWarning: BNNSGraphMessageLevel

A constant that specifies warning message types.

var BNNSGraphMessageLevelError: BNNSGraphMessageLevel

A constant that specifies error message types.

var BNNSGraphMessageLevelUnsupported: BNNSGraphMessageLevel

A constant that specifies unsupported function message types.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying a graph’s compile-time message callback

func BNNSGraphCompileOptionsSetMessageLogMask(bnns_graph_compile_options_t, UInt32)

Sets the mask for compile-time messages.

func BNNSGraphContextSetMessageLogMask(bnns_graph_context_t, UInt32) -> Int32

Sets mask for log messages that are logged (either via `os_log` or the user specified callback)

func BNNSGraphCompileOptionsSetMessageLogCallback(bnns_graph_compile_options_t, bnns_graph_compile_message_fn_t, UnsafeMutablePointer&lt;bnns_user_message_data_t>?)

Specifies a customized callback function that reports compile-time messages.

typealias bnns_graph_compile_message_fn_t

The graph compile-message logging callback function.

struct bnns_user_message_data_t

Additional user-defined logging argument for message-logging callbacks.

