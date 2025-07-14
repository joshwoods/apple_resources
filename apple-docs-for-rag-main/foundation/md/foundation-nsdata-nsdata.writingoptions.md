

- Foundation
- NSData
-  NSData.WritingOptions 

Structure

# NSData.WritingOptions

Options for methods used to write data objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct WritingOptions
```

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var atomic: NSData.WritingOptions

An option to write data to an auxiliary file first and then replace the original file with the auxiliary file when the write completes.

static var withoutOverwriting: NSData.WritingOptions

An option that attempts to write data to a file and fails with an error if the destination file already exists.

static var noFileProtection: NSData.WritingOptions

An option to not encrypt the file when writing it out.

static var completeFileProtection: NSData.WritingOptions

An option to make the file accessible only while the device is unlocked.

static var completeFileProtectionUnlessOpen: NSData.WritingOptions

An option to allow the file to be accessible while the device is unlocked or the file is already open.

static var completeFileProtectionUntilFirstUserAuthentication: NSData.WritingOptions

An option to allow the file to be accessible after a user first unlocks the device.

static var fileProtectionMask: NSData.WritingOptions

An option the system uses when determining the file protection options that the system assigns to the data.

static var atomic: NSData.WritingOptions

An option to write data to an auxiliary file first and then replace the original file with the auxiliary file when the write completes.

static var withoutOverwriting: NSData.WritingOptions

An option that attempts to write data to a file and fails with an error if the destination file already exists.

static var noFileProtection: NSData.WritingOptions

An option to not encrypt the file when writing it out.

static var completeFileProtection: NSData.WritingOptions

An option to make the file accessible only while the device is unlocked.

static var completeFileProtectionUnlessOpen: NSData.WritingOptions

An option to allow the file to be accessible while the device is unlocked or the file is already open.

static var completeFileProtectionUntilFirstUserAuthentication: NSData.WritingOptions

An option to allow the file to be accessible after a user first unlocks the device.

static var fileProtectionMask: NSData.WritingOptions

An option the system uses when determining the file protection options that the system assigns to the data.

### Legacy Constants

static var atomicWrite: NSData.WritingOptions

An option that attempts to write data to an auxiliary file first and then exchange the files.

Deprecated

static var atomicWrite: NSData.WritingOptions

An option that attempts to write data to an auxiliary file first and then exchange the files.

Deprecated

### Entitlements

Data Protection Entitlement

The level of data protection for sensitive user data when an app accesses it on a device.

### Type Properties

static var completeFileProtectionWhenUserInactive: NSData.WritingOptions

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Writing Data to a File

func write(toFile: String, atomically: Bool) -> Bool

Writes the data object’s bytes to the file specified by a given path.

func write(toFile: String, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the file specified by a given path.

func write(to: URL, atomically: Bool) -> Bool

Writes the data object’s bytes to the location specified by a given URL.

func write(to: URL, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the location specified by a given URL.

