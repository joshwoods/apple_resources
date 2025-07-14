

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  getProvisionStatus 

Instance Method

# getProvisionStatus

macOS 10.12+

``` source
virtual IOReturn getProvisionStatus(IOService *client, UInt64 byteStart, UInt64 byteCount, UInt32 *extentsCount, IOStorageProvisionExtent *extents, IOStorageGetProvisionStatusOptions options);
```

