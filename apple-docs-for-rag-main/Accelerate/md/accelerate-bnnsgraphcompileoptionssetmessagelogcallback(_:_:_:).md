

- Accelerate
-  BNNSGraphCompileOptionsSetMessageLogCallback(\_:\_:\_:) 

Function

# BNNSGraphCompileOptionsSetMessageLogCallback(\_:\_:\_:)

Specifies a customized callback function that reports compile-time messages.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphCompileOptionsSetMessageLogCallback(
    _ options: bnns_graph_compile_options_t,
    _ log_callback: bnns_graph_compile_message_fn_t,
    _ additional_logging_arguments: UnsafeMutablePointer?
)
```

## Parameters 

`options`  

The compilation options object.

`log_callback`  

The message-logging callback function.

`additional_logging_arguments`  

Additional data for the message-logging functions that BNNS passes unaltered to the callback function.

## Discussion

If you don’t specify this callback, default callback functions log messages to os_log.

The following code adds a custom graph compile message callback function that prints BNNSGraphMessageLevelInfo level messages to the console:

```
let options = BNNSGraphCompileOptionsMakeDefault()
defer {
    BNNSGraphCompileOptionsDestroy(options)
}

BNNSGraphCompileOptionsSetMessageLogMask(options, BNNSGraphMessageLevelInfo.rawValue)
BNNSGraphCompileOptionsSetMessageLogCallback(options, messageLogCallback, nil)

func messageLogCallback(msg_level: BNNSGraphMessageLevel,
                        error_msg: UnsafePointer,
                        source_location: UnsafePointer?,
                        user_message_data_t:UnsafeMutablePointer?) {

    print(NSString(cString: error_msg, encoding: NSUTF8StringEncoding) ?? "")
    if let source_location = source_location {
        print(NSString(cString: source_location, encoding: NSUTF8StringEncoding) ?? "")
    }
}
```

## See Also

### Specifying a graph’s compile-time message callback

func BNNSGraphCompileOptionsSetMessageLogMask(bnns_graph_compile_options_t, UInt32)

Sets the mask for compile-time messages.

func BNNSGraphContextSetMessageLogMask(bnns_graph_context_t, UInt32) -> Int32

Sets mask for log messages that are logged (either via `os_log` or the user specified callback)

struct BNNSGraphMessageLevel

Constants that specify the mask for compile-time messages.

typealias bnns_graph_compile_message_fn_t

The graph compile-message logging callback function.

struct bnns_user_message_data_t

Additional user-defined logging argument for message-logging callbacks.

