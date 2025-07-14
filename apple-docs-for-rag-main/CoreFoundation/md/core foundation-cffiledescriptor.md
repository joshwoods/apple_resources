

- Core Foundation
-  CFFileDescriptor 

Class

# CFFileDescriptor

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFFileDescriptor
```

## Overview

The CFFileDescriptor provides an opaque type to monitor file descriptors for read and write activity via CFRunLoop.

You use CFFileDescriptor to monitor file descriptors for read and write activity via CFRunLoop using callbacks. Each call back is one-shot, and must be re-enabled if you want to get another one.

You can re-enable the callback in the callback function itself, but you must completely service the file descriptor before doing so. For example, if you create a CFFileDescriptor for a pipe and get a callback because there are bytes to be read, then if you don’t read all of the bytes but nevertheless re-enable the CFFileDescriptor for read activity, you’ll get called back again immediately.

You can monitor kqueue file descriptors for read activity to find out when an event the kqueue is filtering for has occurred. You are responsible for understanding the use of the kevent() API and inserting and removing filters from the kqueue file descriptor yourself.

The following example takes a UNIX process ID as argument, and watches up to 20 seconds, and reports if the process terminates in that time:

```
// cc test.c -framework CoreFoundation -O
#include 
#include 
#include 
static void noteProcDeath(CFFileDescriptorRef fdref, CFOptionFlags callBackTypes, void *info) {
    struct kevent kev;
    int fd = CFFileDescriptorGetNativeDescriptor(fdref);
    kevent(fd, NULL, 0, &kev, 1, NULL);
    // take action on death of process here
    printf("process with pid '%u' died\n", (unsigned int)kev.ident);
    CFFileDescriptorInvalidate(fdref);
    CFRelease(fdref); // the CFFileDescriptorRef is no longer of any use in this example
}
// one argument, an integer pid to watch, required
int main(int argc, char *argv[]) {
    if (argc 

## Topics

### Creating a CFFileDescriptor

func CFFileDescriptorCreate(CFAllocator!, CFFileDescriptorNativeDescriptor, Bool, CFFileDescriptorCallBack!, UnsafePointer&lt;CFFileDescriptorContext>!) -> CFFileDescriptor!

Creates a new CFFileDescriptor.

### Getting Information About a File Descriptor

func CFFileDescriptorGetNativeDescriptor(CFFileDescriptor!) -> CFFileDescriptorNativeDescriptor

Returns the native file descriptor for a given CFFileDescriptor.

func CFFileDescriptorIsValid(CFFileDescriptor!) -> Bool

Returns a Boolean value that indicates whether the native file descriptor for a given CFFileDescriptor is valid.

func CFFileDescriptorGetContext(CFFileDescriptor!, UnsafeMutablePointer&lt;CFFileDescriptorContext>!)

Gets the context for a given CFFileDescriptor.

### Invalidating a File Descriptor

func CFFileDescriptorInvalidate(CFFileDescriptor!)

Invalidates a CFFileDescriptor object.

### Managing Callbacks

func CFFileDescriptorEnableCallBacks(CFFileDescriptor!, CFOptionFlags)

Enables callbacks for a given CFFileDescriptor.

func CFFileDescriptorDisableCallBacks(CFFileDescriptor!, CFOptionFlags)

Disables callbacks for a given CFFileDescriptor.

### Creating a Run Loop Source

func CFFileDescriptorCreateRunLoopSource(CFAllocator!, CFFileDescriptor!, CFIndex) -> CFRunLoopSource!

Creates a new runloop source for a given CFFileDescriptor.

### Getting the CFFileDescriptor Type ID

func CFFileDescriptorGetTypeID() -> CFTypeID

Returns the type identifier for the CFFileDescriptor opaque type.

### Data Types

typealias CFFileDescriptorNativeDescriptor

Defines a type for the native file descriptor.

typealias CFFileDescriptorCallBack

Defines a structure for a callback for a CFFileDescriptor.

struct CFFileDescriptorContext

Defines a structure for the context of a CFFileDescriptor.

### Constants

Callback Identifiers

Constants that identify the read and write callbacks.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

