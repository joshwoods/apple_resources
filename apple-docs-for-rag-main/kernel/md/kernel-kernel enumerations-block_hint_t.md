

- Kernel
- Kernel Enumerations
-  block_hint_t 

Enumeration

# block_hint_t

macOS 10.12.4+

``` source
typedef enum thread_snapshot_wait_flags : unsigned char {
    ...
} block_hint_t;
```

## Topics

### Constants

kThreadWaitKernelMutex

kThreadWaitKernelRWLockRead

kThreadWaitKernelRWLockUpgrade

kThreadWaitKernelRWLockWrite

kThreadWaitNone

kThreadWaitPThreadCondVar

kThreadWaitPThreadMutex

kThreadWaitPThreadRWLockRead

kThreadWaitPThreadRWLockWrite

kThreadWaitParkedWorkQueue

kThreadWaitPortReceive

kThreadWaitPortSend

kThreadWaitPortSendInTransit

kThreadWaitPortSetReceive

kThreadWaitSemaphore

kThreadWaitUserLock

kThreadWaitCompressor

kThreadWaitEventlink

kThreadWaitExclaveCore

kThreadWaitExclaveKit

kThreadWaitMappingInProgress

kThreadWaitMemoryBlocked

kThreadWaitOnProcess

kThreadWaitPageBusy

kThreadWaitPageInThrottle

kThreadWaitPagerInit

kThreadWaitPagerReady

kThreadWaitPagingActivity

kThreadWaitPagingInProgress

kThreadWaitParkedBoundWorkQueue

kThreadWaitSleepWithInheritor

kThreadWaitWorkloopSyncWait

