

- Kernel
- Deprecated Symbols
-  mbuf_inbound_modified Deprecated

Function

# mbuf_inbound_modified

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_inbound_modified(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf that has been modified.

## Discussion

This function will clear the checksum flags to indicate that a hardware checksum should not be used. Any filter modifying data should call this function on an mbuf before passing the packet up the stack. If a filter modifies a packet in a way that affects any checksum, the filter is responsible for either modifying the checksum to compensate for the changes or verifying the checksum before making the changes and then modifying the data and calculating a new checksum only if the original checksum was valid.

