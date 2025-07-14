

- Network
-  nw_framer_start_result_ready 

Global Variable

# nw_framer_start_result_ready

The protocol is immediately ready to send and receive data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
var nw_framer_start_result_ready: nw_framer_start_result_t { get }
```

## See Also

### Start Results

var nw_framer_start_result_will_mark_ready: nw_framer_start_result_t

The protocol will perform a handshake, preventing the overall connection from becoming ready until nw_framer_mark_ready(_:) is called.

