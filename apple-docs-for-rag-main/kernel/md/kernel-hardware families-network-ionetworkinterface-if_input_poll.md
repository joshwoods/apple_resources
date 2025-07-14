

- Kernel
- Hardware Families
- Network
- IONetworkInterface
-  if_input_poll 

Type Method

# if_input_poll

macOS 10.11.4+

``` source
static void if_input_poll(ifnet_t ifp, uint32_t flags, uint32_t max_count, mbuf_t *first_packet, mbuf_t *last_packet, uint32_t *cnt, uint32_t *len);
```

