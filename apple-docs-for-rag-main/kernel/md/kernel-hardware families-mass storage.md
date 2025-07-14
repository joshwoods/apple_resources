

- Kernel
- Hardware Families
-  Mass Storage 

API Collection

# Mass Storage

Implement a driver that communicates with CD, DVD, or other mass storage devices.

## Topics

### Drivers

IOBDBlockStorageDriver

IODVDBlockStorageDriver

IOCDBlockStorageDriver

IOBlockStorageDriver

The common base class for generic block storage drivers.

IOStorage

The common base class for mass storage objects.

### Interfaces

IODVDServices

IOBDBlockStorageDevice

The IOBDBlockStorageDevice class is a generic BD block storage device abstraction.

IODVDBlockStorageDevice

The IODVDBlockStorageDevice class is a generic DVD block storage device abstraction.

IOCompactDiscServices

IOBDMediaBSDClient

IOMediaBSDClient

### Devices

IOBlockStorageServices

IOCDBlockStorageDevice

The IOCDBlockStorageDevice class is a generic CD block storage device abstraction.

IOBDServices

IOBlockStorageDevice

A generic block storage device abstraction.

### Data Storage

IOCDMedia

The IOCDMedia class is a random-access disk device abstraction for CDs.

IOBDMedia

The IOBDMedia class is a random-access disk device abstraction for BDs.

IOMedia

A random-access disk device abstraction.

IOCDMediaBSDClient

IOCDPartitionScheme

IODVDMedia

The IODVDMedia class is a random-access disk device abstraction for DVDs.

IODVDMediaBSDClient

### Schemes

IOAppleLabelScheme

IOApplePartitionScheme

IOFDiskPartitionScheme

IOGUIDPartitionScheme

IOPartitionScheme

The common base class for all partition scheme objects.

IOFilterScheme

The common base class for all filter scheme objects.

### Data

CD Data Structures

DVD Data Structures

## See Also

### Interfaces

Audio

Implement a driver that interacts with audio hardware.

Graphics and Displays

Implement a driver that interacts with graphics and video hardware.

HID

Implement a driver that interacts with human interface devices, such as mice and keyboards.

Network

Implement a driver that interacts with network interfaces such as Ethernet adaptors.

SCSI

Implement a driver that supports Small Computer System Interface (SCSI) protocols.

