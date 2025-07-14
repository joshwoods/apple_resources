

- Kernel
- Hardware Families
- Network
- IOPacketQueue
-  IOPacketQueueDefaultCapacity 

# IOPacketQueueDefaultCapacity

Describes the default capacity of the queue object.

``` source
static const UInt32 IOPacketQueueDefaultCapacity = 100;
```

## Overview

The capacity is only observed by the enqueue() method. Therefore, it is possible for the size of the queue to exceed its capacity when other methods, such as prepend(), are used to add packets to the queue.

