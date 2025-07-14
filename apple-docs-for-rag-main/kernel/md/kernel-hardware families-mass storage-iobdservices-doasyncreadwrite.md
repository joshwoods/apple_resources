

- Kernel
- Hardware Families
- Mass Storage
- IOBDServices
-  doAsyncReadWrite 

Instance Method

# doAsyncReadWrite

macOS 10.15.2+

``` source
virtual IOReturn doAsyncReadWrite(IOMemoryDescriptor *buffer, UInt64 block, UInt64 nblks, IOStorageAttributes *attributes, IOStorageCompletion *completion);
```

