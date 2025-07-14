

- CloudKit
- CKRecord
-  CKRecord.SystemFieldKey 

Enumeration

# CKRecord.SystemFieldKey

Possible values for types of system field keys on records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
enum SystemFieldKey
```

## Overview

Use the values share and parent when creating an NSPredicate for a CKQuery to reference a record’s share or parent property, respectively.

## Topics

### Types of Shared Records

static let parent: CKRecord.FieldKey

A value that represents the parent property of a record.

static let share: CKRecord.FieldKey

A value that represents the share property of a record.

### Type Properties

static var creationDate: CKRecord.FieldKey

static var creatorUserRecordID: CKRecord.FieldKey

static var lastModifiedUserRecordID: CKRecord.FieldKey

static var modificationDate: CKRecord.FieldKey

static var recordID: CKRecord.FieldKey

## See Also

### Sharing Records

var parent: CKRecord.Reference?

A reference to the record’s parent record.

var share: CKRecord.Reference?

A reference to the share object that determines the share status of the record.

class Reference

A relationship between two records in a record zone.

func setParent(CKRecord?)

Creates and sets a reference object for a parent from its record.

func setParent(CKRecord.ID?)

Creates and sets a reference object for a parent from the parent’s record ID.

