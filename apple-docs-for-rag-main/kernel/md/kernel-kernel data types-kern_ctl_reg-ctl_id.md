

- Kernel
- Kernel Data Types
- kern_ctl_reg
-  ctl_id 

Instance Property

# ctl_id

The control ID may be dynamically assigned or it can be a 32-bit creator code assigned by DTS. For a DTS assigned creator code the CTL_FLAG_REG_ID_UNIT flag must be set. For a dynamically assigned control ID, do not set the CTL_FLAG_REG_ID_UNIT flag. The value of the dynamically assigned control ID is set to this field when the registration succeeds.

macOS 10.13+

``` source
u_int32_t ctl_id;
```

## See Also

### Fields

ctl_name

A Bundle ID string of up to MAX_KCTL_NAME bytes (including the ending zero). This string should not be empty.

ctl_unit

A separate unit number to register multiple units that share the same control ID with DTS assigned creator code when the CTL_FLAG_REG_ID_UNIT flag is set. This field is ignored for a dynamically assigned control ID.

ctl_flags

CTL_FLAG_PRIVILEGED and/or CTL_FLAG_REG_ID_UNIT.

ctl_sendsize

Override the default send size. If set to zero, the default send size will be used, and this default value is set to this field to be retrieved by the caller.

ctl_recvsize

Override the default receive size. If set to zero, the default receive size will be used, and this default value is set to this field to be retrieved by the caller.

ctl_connect

Specify the function to be called whenever a client connects to the kernel control. This field must be specified.

ctl_disconnect

Specify a function to be called whenever a client disconnects from the kernel control.

ctl_send

Specify a function to handle data send from the client to the kernel control.

ctl_setopt

Specify a function to handle set socket option operations for the kernel control.

ctl_getopt

Specify a function to handle get socket option operations for the kernel control.

