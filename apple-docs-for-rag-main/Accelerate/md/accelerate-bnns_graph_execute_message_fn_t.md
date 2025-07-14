

- Accelerate
-  bnns_graph_execute_message_fn_t 

Type Alias

# bnns_graph_execute_message_fn_t

The graph execute-message logging callback function.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
typealias bnns_graph_execute_message_fn_t = (BNNSGraphMessageLevel, UnsafePointer, UnsafePointer?, UnsafeMutablePointer?) -> Void
```

## See Also

### Specifying a context’s execute-time message callback

func BNNSGraphContextSetMessageLogCallback(bnns_graph_context_t, bnns_graph_execute_message_fn_t, UnsafeMutablePointer&lt;bnns_user_message_data_t>?) -> Int32

Specifies a customized callback function that reports execution-time messages.

struct BNNSGraphMessageLevel

Constants that specify the mask for compile-time messages.

struct bnns_user_message_data_t

Additional user-defined logging argument for message-logging callbacks.

