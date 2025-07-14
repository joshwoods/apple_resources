

- Kernel
- Hardware Families
- Mass Storage
- IODVDBlockStorageDriver
-  reportKey 

Instance Method

# reportKey

macOS 15.4+

``` source
virtual IOReturn reportKey(IOMemoryDescriptor *buffer, const DVDKeyClass keyClass, const UInt32 lba, const UInt8 blockCount, const UInt8 agid, const DVDKeyFormat keyFormat);
```

