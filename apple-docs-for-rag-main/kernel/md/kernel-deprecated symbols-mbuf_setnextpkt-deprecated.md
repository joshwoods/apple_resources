

- Kernel
- Deprecated Symbols
-  mbuf_setnextpkt Deprecated

Function

# mbuf_setnextpkt

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_setnextpkt(mbuf_t mbuf, mbuf_t nextpkt);
```

## Parameters 

`mbuf`  

The mbuf.

`nextpkt`  

The new next packet.

## Discussion

Sets the next packet attached to this mbuf.

