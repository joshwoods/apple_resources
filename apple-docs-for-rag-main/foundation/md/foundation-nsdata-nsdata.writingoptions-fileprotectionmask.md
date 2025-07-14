

- Foundation
- NSData
- NSData.WritingOptions
-  fileProtectionMask 

Type Property

# fileProtectionMask

An option the system uses when determining the file protection options that the system assigns to the data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var fileProtectionMask: NSData.WritingOptions { get }
```

## See Also

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

