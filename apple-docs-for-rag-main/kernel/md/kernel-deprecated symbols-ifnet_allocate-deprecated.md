

- Kernel
- Deprecated Symbols
-  ifnet_allocate Deprecated

Function

# ifnet_allocate

macOS 10.4–10.15.4Deprecated

``` source
errno_t ifnet_allocate(const struct ifnet_init_params *init, ifnet_t *interface);
```

## Parameters 

`init`  

The initial values for the interface. These values can not be changed after the interface has been allocated.

`interface`  

The interface allocated upon success.

## Return Value

May return ENOMEM if there is insufficient memory or EEXIST if an interface with the same uniqueid and family has already been allocated and is in use.

## Discussion

Allocate an ifnet_t with an initial refcount of 1. Many parts of the stack do not properly refcount the ifnet_t. In order to avoid freeing the ifnet_t while some parts of the stack may contain a reference to it, the ifnet_ts are only recycled, never freed. A unique id is used to try and recycle the same ifnet_t when allocating an interface. For example, for an ethernet interface, the hardware address of the ethernet card is usually used for the uniqueid. If a PC Card is removed and inserted again, if the ethernet address of the PC card is used, the same ifnet_t will be used for the card the second time it is inserted. In the future, when the ifnet_t is correctly refcounted by all of the stack, the interfaces may be freed and the unique ids ignored.

## See Also

### Network Kernel Extensions

sock_acceptDeprecated

sock_bindDeprecated

sock_closeDeprecated

sock_connectDeprecated

sock_getpeernameDeprecated

sock_getsocknameDeprecated

sock_getsockoptDeprecated

sock_gettypeDeprecated

sock_inject_data_inDeprecated

sock_inject_data_outDeprecated

sock_ioctlDeprecated

sock_isconnectedDeprecated

sock_isnonblockingDeprecated

sock_listenDeprecated

sock_receiveDeprecated

sock_receivembufDeprecated

sock_sendDeprecated

sock_sendmbufDeprecated

sock_setprivDeprecated

sock_setsockoptDeprecated

sock_shutdownDeprecated

sock_socketDeprecated

sockopt_copyinDeprecated

sockopt_copyoutDeprecated

sockopt_directionDeprecated

sockopt_levelDeprecated

sockopt_nameDeprecated

sockopt_valsizeDeprecated

ifaddr_addressDeprecated

ifaddr_address_familyDeprecated

ifaddr_dstaddressDeprecated

ifaddr_findbestforaddrDeprecated

ifaddr_ifnetDeprecated

ifaddr_netmaskDeprecated

ifaddr_referenceDeprecated

ifaddr_releaseDeprecated

ifaddr_withaddrDeprecated

ifaddr_withdstaddrDeprecated

ifaddr_withnetDeprecated

ifaddr_withrouteDeprecated

iflt_attachDeprecated

iflt_detachDeprecated

ifmaddr_addressDeprecated

ifmaddr_ifnetDeprecated

ifmaddr_lladdressDeprecated

ifmaddr_referenceDeprecated

ifmaddr_releaseDeprecated

ifnet_add_multicastDeprecated

ifnet_addrlenDeprecated

ifnet_attachDeprecated

ifnet_attach_protocolDeprecated

ifnet_attach_protocol_v2Deprecated

ifnet_baudrateDeprecated

ifnet_capabilities_enabledDeprecated

ifnet_capabilities_supportedDeprecated

ifnet_detachDeprecated

ifnet_detach_protocolDeprecated

ifnet_eventDeprecated

ifnet_familyDeprecated

ifnet_find_by_nameDeprecated

ifnet_flagsDeprecated

ifnet_free_address_listDeprecated

ifnet_free_multicast_listDeprecated

ifnet_get_address_listDeprecated

ifnet_get_address_list_familyDeprecated

ifnet_get_link_mib_dataDeprecated

ifnet_get_link_mib_data_lengthDeprecated

ifnet_get_multicast_listDeprecated

ifnet_get_tso_mtuDeprecated

ifnet_get_wake_flagsDeprecated

ifnet_hdrlenDeprecated

ifnet_indexDeprecated

ifnet_inputDeprecated

ifnet_interface_family_findDeprecated

ifnet_ioctlDeprecated

ifnet_lastchangeDeprecated

ifnet_list_freeDeprecated

ifnet_list_getDeprecated

ifnet_lladdr_copy_bytesDeprecated

ifnet_llbroadcast_copy_bytesDeprecated

ifnet_metricDeprecated

ifnet_mtuDeprecated

ifnet_nameDeprecated

ifnet_offloadDeprecated

ifnet_outputDeprecated

ifnet_output_rawDeprecated

ifnet_referenceDeprecated

ifnet_releaseDeprecated

ifnet_remove_multicastDeprecated

ifnet_resolve_multicastDeprecated

ifnet_set_addrlenDeprecated

ifnet_set_baudrateDeprecated

ifnet_set_capabilities_enabledDeprecated

ifnet_set_capabilities_supportedDeprecated

ifnet_set_flagsDeprecated

ifnet_set_hdrlenDeprecated

ifnet_set_link_mib_dataDeprecated

ifnet_set_lladdrDeprecated

ifnet_set_metricDeprecated

ifnet_set_mtuDeprecated

ifnet_set_offloadDeprecated

ifnet_set_promiscuousDeprecated

ifnet_set_statDeprecated

ifnet_set_tso_mtuDeprecated

ifnet_set_wake_flagsDeprecated

ifnet_softcDeprecated

ifnet_statDeprecated

ifnet_stat_incrementDeprecated

ifnet_stat_increment_inDeprecated

ifnet_stat_increment_outDeprecated

ifnet_touch_lastchangeDeprecated

ifnet_typeDeprecated

ifnet_unitDeprecated

