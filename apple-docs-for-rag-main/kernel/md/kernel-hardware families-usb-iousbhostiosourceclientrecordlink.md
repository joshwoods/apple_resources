

- Kernel
- Hardware Families
- USB
-  IOUSBHostIOSourceClientRecordLink 

Structure

# IOUSBHostIOSourceClientRecordLink

A structure that represents a USB host input/output source client record entry.

macOS 10.13+

``` source
typedef struct IOUSBHostIOSourceClientRecordLink {
    ...
} IOUSBHostIOSourceClientRecordLink;
```

## Topics

### Getting the Properties

le_next

The pointer to the next USB host input/output source client record.

le_prev

The pointer to the previous USB host input/output source client record.

## See Also

### Device Communication

Building a Simple USB Driver

Set up and load a driver that logs output to the Console app.

IOUSBHostIOSourceClientRecordList

A structure that represents a list of USB host input/output source client records.

