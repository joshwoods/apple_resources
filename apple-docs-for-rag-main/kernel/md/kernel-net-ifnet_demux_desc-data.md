

- Kernel
- net
- ifnet_demux_desc
-  data 

Instance Property

# data

A pointer to an entry of type (i.e. pointer to 0x0800).

macOS 10.6+

``` source
void *data;
```

## See Also

### Fields

type

The type of identifier data (i.e. ETHER_DESC_ETYPE2)

datalen

The number of bytes of data used to describe the packet.

