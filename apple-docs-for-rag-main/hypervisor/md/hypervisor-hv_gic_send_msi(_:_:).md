

- Hypervisor
-  hv_gic_send_msi(\_:\_:) 

Function

# hv_gic_send_msi(\_:\_:)

Sends a message signaled interrupt (MSI).

macOS 15.0+

``` source
func hv_gic_send_msi(
    _ address: hv_ipa_t,
    _ intid: UInt32
) -> hv_return_t
```

## Parameters 

`address`  

The guest physical address for message-based shared peripheral interrupts (SPI).

`intid`  

The Interrupt identifier for the message based SPI.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## Discussion

Use the address of the HV_GIC_REG_GICM_SET_SPI_NSR register in the MSI frame.

## See Also

### Sending interrupts

func hv_gic_set_spi(UInt32, Bool) -> hv_return_t

Triggers a shared peripheral interrupt (SPI).

