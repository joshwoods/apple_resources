

- AppKit
- NSSharingService
-  NSSharingService.CloudKitOptions 

Structure

# NSSharingService.CloudKitOptions

Constants that describe how a participant can configure a CloudKit share.

macOS 10.12+

``` source
struct CloudKitOptions
```

## Topics

### Creating CloudKit Options

init(rawValue: UInt)

Creates a set of CloudKit options using the specified raw value.

### CloudKit Options

static var allowPrivate: NSSharingService.CloudKitOptions

An option that allows the participant to privately distribute the share to other iCloud users.

static var allowPublic: NSSharingService.CloudKitOptions

An option that allows the participant to publicly distribute the share to other iCloud users.

static var allowReadOnly: NSSharingService.CloudKitOptions

An option that allows the participant to grant other participants read-only permissions.

static var allowReadWrite: NSSharingService.CloudKitOptions

An option that allows the participant to grant other participants read-write permissions.

static var standard: NSSharingService.CloudKitOptions

An option that allows the participant to configure the share with a standard set of options.

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

### Managing the Cloud-Sharing Service

func sharingService(NSSharingService, didCompleteForItems: [Any], error: (any Error)?)

Tells the delegate when the cloud-sharing service completes.

func sharingService(NSSharingService, didSave: CKShare)

Tells the delegate when the cloud-sharing service saves the CloudKit share.

func sharingService(NSSharingService, didStopSharing: CKShare)

Tells the delegate when the user stops sharing the CloudKit share.

func options(for: NSSharingService, share: NSItemProvider) -> NSSharingService.CloudKitOptions

Asks the delegate for the participant options for the cloud-sharing service.

