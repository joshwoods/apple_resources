

- Kernel
- net
- ifnet_demux_desc
-  datalen 

Instance Property

# datalen

The number of bytes of data used to describe the packet.

macOS 10.6+

``` source
u_int32_t datalen;
```

## See Also

### Fields

type

The type of identifier data (i.e. ETHER_DESC_ETYPE2)

data

A pointer to an entry of type (i.e. pointer to 0x0800).

