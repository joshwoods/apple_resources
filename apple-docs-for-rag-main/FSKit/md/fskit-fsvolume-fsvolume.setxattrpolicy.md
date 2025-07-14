

- FSKit
- FSVolume
-  FSVolume.SetXattrPolicy 

Enumeration

# FSVolume.SetXattrPolicy

Flags to specify the policy when setting extended file attributes.

macOS 15.4+

``` source
enum SetXattrPolicy
```

## Topics

### Declaring a policy

case alwaysSet

Set the value, regardless of previous state.

case mustCreate

Set the value, but fail if the extended attribute already exists.

case mustReplace

Set the value, but fail if the extended attribute doesn’t already exist.

case delete

Delete the value, failing if the extended attribute doesn’t exist.

### Initializers

init?(rawValue: UInt)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reading and writing

func getXattr(named: FSFileName, of: FSItem, replyHandler: (Data?, (any Error)?) -> Void)

Gets the specified extended attribute of the given item.

**Required**

func listXattrs(of: FSItem, replyHandler: ([FSFileName]?, (any Error)?) -> Void)

Gets the list of extended attributes currently set on the given item.

**Required**

func setXattr(named: FSFileName, to: Data?, on: FSItem, policy: FSVolume.SetXattrPolicy, replyHandler: ((any Error)?) -> Void)

Sets the specified extended attribute data on the given item.

**Required**

func supportedXattrNames(for: FSItem) -> [FSFileName]

Returns an array that specifies the extended attribute names the given item supports.

