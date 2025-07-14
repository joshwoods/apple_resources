

- watchOS Release Notes
-  watchOS 9.1 Release Notes 

Article

# watchOS 9.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The watchOS 9.1 SDK provides support to develop watchOS apps for Apple Watch devices running watchOS 9.1. The SDK comes bundled with Xcode 14.1 RC, available from Beta Software Downloads. For information on the compatibility requirements for Xcode 14.1, see Xcode 14.1 Release Notes.

### Memory Allocation

#### Known Issues

- The system memory allocator `free` operation zeroes out most deallocated blocks in watchOS 9.1 beta or later. Invalid accesses to free memory might result in new crashes or corruption, including:

  - Read-after-free bugs that previously observed the old contents of a block may now observe zeroes instead

  - Write-after-free bugs may now cause subsequent calls to `calloc` to return non-zero memory

To debug these issues, use Address Sanitizer and Guard Malloc (see `libgmalloc(3)`). (97449075)

## See Also

### watchOS 9

watchOS 9.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 9.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 9.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 9.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 9.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 9 Release Notes

Update your apps to use new features, and test your apps against API changes.

