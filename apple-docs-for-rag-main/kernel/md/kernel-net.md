

- Kernel
-  net 

API Collection

# net

Access network-related utilities.

## Topics

### Address Resolution

inet_arp_handle_input

inet_arp_init_ifaddr

inet_arp_lookup

### bpf

bpf_attach

bpf_tap_in

bpf_tap_out

bpfattach

### ether

ether_family_init

ether_add_proto

ether_del_proto

ether_demux

ether_frameout

ether_ioctl

ether_check_multi

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_attach_proto_param_v2

ifnet_check_multi

ifnet_del_proto_func

ifnet_demux_desc

ifnet_demux_func

ifnet_detached_func

ifnet_event_func

ifnet_family_t

Storage type for the interface family.

ifnet_framer_func

ifnet_init_params

ifnet_ioctl_func

ifnet_offload_t

Flags indicating the offload support of the interface.

ifnet_output_func

ifnet_set_bpf_tap

ifnet_stat_increment_param

ifnet_stats_param

ifnet_t

## See Also

### BSD

architecture

Access machine-level and architectural information about the current platform.

bsm

Audit resource usage on the system.

hfs

Access HFS file-system data structures.

kern

Access kernel-level interfaces including clock, task, kernel extension, lock, and compression utilities.

Math

Perform mathematical operations and manipulate integer, float, and double values.

miscfs

Access device nodes and other file-system entities.

Strings

Compare, convert, and catenate strings and access the resulting content of those strings.

sys

Access general system utilities for time, file systems, and system information.

vfs

Access the virtual file-system interfaces.

vm

Interact with the virtual memory system.

