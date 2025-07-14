

- System
- FileDescriptor
- FileDescriptor.OpenOptions
-  eventOnly 

Type Property

# eventOnly

Indicates that opening the file monitors a file for changes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var eventOnly: FileDescriptor.OpenOptions { get }
```

## Mentioned in 

Adopting Swift File Options

## Discussion

Specify this option when opening a file for event notifications, such as a file handle returned by the `kqueue(2)` function, rather than for reading or writing. Files opened with this option don’t prevent their containing volume from being unmounted.

The corresponding C constant is `O_EVTONLY`.

## See Also

### Specifying Options

static var append: FileDescriptor.OpenOptions

Indicates that each write operation appends to the file.

static var closeOnExec: FileDescriptor.OpenOptions

Indicates that executing a program closes the file.

static var create: FileDescriptor.OpenOptions

Indicates that opening the file creates the file if it doesn’t exist.

static var exclusiveCreate: FileDescriptor.OpenOptions

Indicates that opening the file creates the file, expecting that it doesn’t exist.

static var exclusiveLock: FileDescriptor.OpenOptions

Indicates that opening the file atomically obtains an exclusive lock.

static var noFollow: FileDescriptor.OpenOptions

Indicates that opening the file doesn’t follow symlinks.

static var nonBlocking: FileDescriptor.OpenOptions

Indicates that opening the file doesn’t wait for the file or device to become available.

static var sharedLock: FileDescriptor.OpenOptions

Indicates that opening the file atomically obtains a shared lock on the file.

static var symlink: FileDescriptor.OpenOptions

Indicates that opening the file opens symbolic links instead of following them.

static var truncate: FileDescriptor.OpenOptions

Indicates that opening the file truncates the file if it exists.

