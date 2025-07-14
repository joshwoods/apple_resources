

- Foundation
- URLResourceKey
-  labelColorKey 

Type Property

# labelColorKey

The resource’s label color, returned as an `NSColor` object, or `nil` if the resource has no label color (read-only).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let labelColorKey: URLResourceKey
```

## See Also

### Other resource keys

static let keysOfUnsetValuesKey: URLResourceKey

Key for the resource properties that have not been set after the setResourceValues(_:) method returns an error, returned as an array of `NSString` objects.

static let quarantinePropertiesKey: URLResourceKey

static let addedToDirectoryDateKey: URLResourceKey

The time at which the resource’s was created or renamed into or within its parent directory, returned as an `NSDate`. Inconsistent behavior may be observed when this attribute is requested on hard-linked items. This property is not supported by all volumes. (read-only)

static let attributeModificationDateKey: URLResourceKey

The time at which the resource’s attributes were most recently modified, returned as an `NSDate` object if the volume supports attribute modification dates, or `nil` if attribute modification dates are unsupported (read-only).

static let contentAccessDateKey: URLResourceKey

The time at which the resource was most recently accessed.

static let contentModificationDateKey: URLResourceKey

The time at which the resource was most recently modified.

static let creationDateKey: URLResourceKey

The time at which the resource was created.

static let customIconKey: URLResourceKey

The icon stored with the resource, returned as an `NSImage` object, or `nil` if the resource has no custom icon.

static let documentIdentifierKey: URLResourceKey

The document identifier returned as an `NSNumber` (read-only).

static let effectiveIconKey: URLResourceKey

The resource’s normal icon, returned as an `NSImage` object (read-only).

static let generationIdentifierKey: URLResourceKey

An opaque generation identifier, returned as an `id ` (read-only)

static let hasHiddenExtensionKey: URLResourceKey

Key for determining whether the resource’s extension is normally removed from its localized name, returned as a Boolean `NSNumber` object (read-write).

static let isExcludedFromBackupKey: URLResourceKey

A key for indicating whether the system excludes the resource from all backups of app data.

static let isExecutableKey: URLResourceKey

Key for determining whether the current process (as determined by the EUID) can execute the resource (if it is a file) or search the resource (if it is a directory), returned as a Boolean `NSNumber` object (read-only).

static let isHiddenKey: URLResourceKey

Key for determining whether the resource is normally not displayed to users, returned as a Boolean `NSNumber` object (read-write).

