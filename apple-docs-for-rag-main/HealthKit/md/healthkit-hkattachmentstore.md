

- HealthKit
-  HKAttachmentStore 

Class

# HKAttachmentStore

The access point for attachments associated with samples in the HealthKit store.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKAttachmentStore
```

## Overview

Use an HKAttachmentStore object to manage attachments for samples that your app has saved to the HealthKit store.

## Topics

### Creating an attachment store

init(healthStore: HKHealthStore)

Creates an attachment store for the provided HealthKit store.

### Adding attachments

func addAttachment(to: HKObject, name: String, contentType: UTType, url: URL, metadata: [String : Any]) async throws -> HKAttachment

Asynchronously adds an attachment to the specified object.

func addAttachment(to: HKObject, name: String, contentType: UTType, url: URL, metadata: [String : Any], completion: (HKAttachment?, (any Error)?) -> Void)

Adds an attachment to the specified object.

### Accessing attachments

func getAttachments(for: HKObject, completion: ([HKAttachment]?, (any Error)?) -> Void)

Returns all the attachments for the specified object.

func dataReader(for: HKAttachment) -> HKAttachmentDataReader

Returns a data reader for the attachment.

func getData(for: HKAttachment, completion: (Data?, (any Error)?) -> Void) -> Progress

Returns an attachment’s data.

func streamData(for: HKAttachment, dataHandler: (Data?, (any Error)?, Bool) -> Void) -> Progress

Asynchronously returns the attachment’s data.

### Removing attachments

func removeAttachment(HKAttachment, from: HKObject, completion: (Bool, (any Error)?) -> Void)

Removes the specified attachment.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Attachments

class HKAttachment

A file that is attached to a sample in the HealthKit store.

class HKAttachmentDataReader

A reader that provides access to an attachment’s data.

