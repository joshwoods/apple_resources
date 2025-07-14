

- Core Data
- Mirroring a Core Data store with CloudKit
-  Reading CloudKit Records for Core Data 

Article

# Reading CloudKit Records for Core Data

Access CloudKit records created from Core Data managed objects.

## Overview

Although your Core Data app interacts primarily with managed objects, you can access a managed object’s CKRecord directly. This is useful if you’re leveraging CloudKit to add features like sharing. You can also use CloudKit JS to access CloudKit records from your web app.

To prevent collision with existing CloudKit record types and reserved names, CloudKit prefixes the CKRecord types and fields it creates for your Core Data entities with `CD_`.

To work with records directly, you need to understand the mappings between entities and record types, attributes and fields, and the ways a record stores relationships.

Note

Core Data doesn’t use CloudKit’s native support for relationships, CKRecord.Reference, because this field limits the number of references to 750, and cannot represent many-to-many relationships. Core Data stores the relationship in CloudKit according to its cardinality (one-to-one, one-to-many, or many-to-many), as described in this article.

### Read Entities from Record Types

CloudKit doesn’t typically support inheritance, so it provides only a single system field, recordType, to hold type information. Core Data stores the name of the *root entity* from the inheritance hierarchy in recordType.

When you initialize a schema, Core Data adds a custom field to the record type, `CD_entityName`, to store the name of the *current entity*.

For example, an entity named `Post` generates the following structure (before adding its attributes), with its `CD_entityName` set to `Post`, and its `recordType` set to `CD_Post`.

```

```

Consider a second entity, `ImagePost`, that inherits from Post.

`ImagePost` generates the following structure (before adding its attributes), with its `CD_entityName` set to `ImagePost`, and its `recordType` set to `CD_Post`.

```

```

Query against recordType when searching against an entity’s inheritance hierarchy. Query against `CD_entityName` when searching for instances of a specific type.

For more information about CloudKit queries, see CKQuery.

### Read Attributes from Fields

When you initialize a schema, Core Data creates fields for each of an entity’s attributes, mapping the attribute name to a field with a key in the form `CD_[attribute.name]`. The field’s type may vary between Core Data and CloudKit.

| Core Data attribute type | `NSManagedObject` attribute type | `CKRecord` attribute type |
|----|----|----|
| `Integer 16` | NSNumber | NSNumber |
| `Integer 32` | NSNumber | NSNumber |
| `Integer 64` | NSNumber | NSNumber |
| `Double` | NSNumber | NSNumber |
| `Float` | NSNumber | NSNumber |
| `Boolean` | NSNumber | NSNumber |
| `Date` | NSDate | NSDate |
| `Decimal` | NSDecimalNumber | NSNumber |
| `UUID` | NSUUID | NSString |
| `URI` | NSURL | NSString |
| `String` | NSString | NSString or CKAsset |
| `Binary Data` | NSData | NSData or CKAsset |
| `Transformable` | NSData | NSData or CKAsset |
| `Undefined` | — | not supported |
| `Object ID` | — | not supported |

All variable length attribute types—String, Binary Data, and Transformable—generate an additional field with a key in the form `CD_[attribute.name]_ckAsset`. If a field’s value grows too large to store within the record size limit of 1MB, Core Data automatically converts the value to an external asset. Core Data transitions between the original field and its asset counterpart transparently during serialization. When inspecting a CloudKit record directly, check the length of the original field’s value; if it is zero, look in the asset field.

For example, an entity named `Post` with String `content` and `title` attributes would generate the following fully materialized record, with pairs of fields for `CD_content and` `CD_content_ckAsset`, and for `CD_title` and `CD_title_ckAsset`.

```
";
    "CD_entityName" = Post;
    "CD_title" = "An example core data string";
    "CD_title_ckAsset" = "";
}, recordType=CD_Post
```

### Read One-to-One Relationships from Fields

One-to-one relationships store foreign keys in both related records, mapping the relationship name to a field with a key in the form `CD_[relationship.name]`. This field stores the foreign key of the related object in the form `CKRecord.recordID.recordName`.

For example, consider a one-to-one relationship between an `ImageData` entity and an `Attachment` entity. In Core Data, the `Attachment` has an `imageData` relationship, and the `ImageData` has an `attachment` relationship.

This one-to-one relationship between `ImageData` and `Attachment` would generate the following CloudKit records.

```

```

The `CD_imageData` field on the `CD_Attachment` contains the foreign key of the image, and the `CD_attachment` field on the `CD_ImageData` contains the foreign key of the attachment.

### Read One-to-Many Relationships from Fields

One-to-many relationships store a foreign key on each record on the many side of the relationship, mapping the relationship name to a field with a key in the form `CD_[relationship name]`. This field stores the foreign key of the related object in the form `CKRecord.recordID.recordName`.

For example, a one-to-many relationship between a single `Post` and multiple `Attachment` instances would generate multiple `CD_Attachment` records. Each record contains the foreign key of the `Post` it belongs to in their `CD_post` field.

```

```

Generated `Post` records don’t contain a reference to their attachments.

### Read Many-to-Many Relationships from CDMR Records

Many-to-many relationships model the join table using a custom Core Data Mirrored Relationship (CDMR) record type.

CloudKit doesn’t support the notion of a join, and it’s inefficient to encode arrays on both records and keep them in sync. Instead, Core Data constructs a CDMR record to accurately and succintly capture all of the criteria of the join.

CDMR records have the following fields.

| CDMR Field | Description |
|----|----|
| `CD_entityNames` | An alphabetically sorted, semicolon-separated list of the entities in the relationship, for example, `“Post:Tag”`. The ordering of this field determines the ordering for all other fields. |
| `CD_recordNames` | The record names of the two related objects, for example, `“CD_Post_F587C290-BC2F-441B-98FC-1357BA89C411:CD_Tag_215FA1E0-6A16-4A2B-BFA2-C13202BE6D50”`, sorted according to the CD_entityNames order. |
| `CD_relationships` | The relationship names, for example, `“tags:posts”`, sorted according to the CD_entityNames order. |

For example, consider a many-to-many relationship between `Tag` and `Post` entities.

The individual `Tag` and `Post` records don’t contain fields for the relationship.

```
";
    "CD_entityName" = Post;
    "CD_title" = "An example core data string";
    "CD_title_ckAsset" = "";
}, recordType=CD_Post>
";
    "CD_entityName" = Tag;
    "CD_name" = "An example core data string";
    "CD_name_ckAsset" = "";
    "CD_uuid" = "51BAFD98-D1F7-472F-95D6-BBF40D7CBD75";
}, recordType=CD_Tag>
```

The relationship between any two `Tag` and `Post` records exists in a third CDMR record. The CDMR record describes the entity type, record name, and Core Data relationship between the `Tag` and `Post`.

```

```

The structure of a CDMR record is carefully designed to occupy the minimum necessary footprint, and to require the least effort to decode and work with, making it usable outside the Core Data framework.

### Access CloudKit Objects

You can access a managed object’s CKRecord directly through its associated context using `record(for:)` for a single record, or `records(for:)` for multiple records. To retrieve the record ID only, use `recordID(for:)`, or `recordIDs(for:)`.

Alternatively, use the class functions recordForManagedObjectID:, recordsForManagedObjectIDs:, recordIDForManagedObjectID:, and `recordIDs(for:)` on NSPersistentCloudKitContainer.

## See Also

### Configuring CloudKit Mirroring

Setting Up Core Data with CloudKit

Set up the classes and capabilities that sync your store to CloudKit.

Creating a Core Data Model for CloudKit

Design a CloudKit-compatible data model and initialize your CloudKit schema.

Syncing a Core Data Store with CloudKit

Synchronize objects between devices, and handle store changes in the user interface.

