

- Accelerate
-  BNNSGraphContextSetMessageLogCallback(\_:\_:\_:) 

Function

# BNNSGraphContextSetMessageLogCallback(\_:\_:\_:)

Specifies a customized callback function that reports execution-time messages.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextSetMessageLogCallback(
    _ context: bnns_graph_context_t,
    _ log_callback_fn: bnns_graph_execute_message_fn_t,
    _ additional_logging_arguments: UnsafeMutablePointer?
) -> Int32
```

## Parameters 

`context`  

The graph context.

`log_callback_fn`  

The message-logging callback function.

`additional_logging_arguments`  

Additional data for the message logging functions that BNNS passes unaltered to the callback function.

## Return Value

`0` on success, nonzero on failure.

## Discussion

The following code adds a custom context execute-message callback function that prints messages to the console:

```
BNNSGraphContextSetMessageLogCallback(context, messageLogCallback, nil)

func messageLogCallback(msg_level: BNNSGraphMessageLevel,
                        error_msg: UnsafePointer,
                        op_info: UnsafePointer?,
                        additional_logging_arguments: UnsafeMutablePointer?) {

    print(NSString(cString: error_msg, encoding: NSUTF8StringEncoding) ?? "")
    if let op_info = op_info {
        print(NSString(cString: op_info, encoding: NSUTF8StringEncoding) ?? "")
    }
}
```

## See Also

### Specifying a context’s execute-time message callback

typealias bnns_graph_execute_message_fn_t

The graph execute-message logging callback function.

struct BNNSGraphMessageLevel

Constants that specify the mask for compile-time messages.

struct bnns_user_message_data_t

Additional user-defined logging argument for message-logging callbacks.

