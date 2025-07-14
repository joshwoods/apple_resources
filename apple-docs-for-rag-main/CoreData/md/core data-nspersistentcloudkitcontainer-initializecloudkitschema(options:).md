

- Core Data
- NSPersistentCloudKitContainer
-  initializeCloudKitSchema(options:) 

Instance Method

# initializeCloudKitSchema(options:)

Creates the CloudKit schema for all stores in the container that manage a CloudKit database.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func initializeCloudKitSchema(options: NSPersistentCloudKitContainerSchemaInitializationOptions = []) throws
```

## Parameters 

`options`  

The options to use when creating the CloudKit schema.

## Discussion

To create the schema, this method creates a set of representative CKRecord instances for all stores in the container that use Core Data with CloudKit, and uploads them to CloudKit. These records have a representative value for every field Core Data might serialize for the specified managed object model. After successfully uploading the records, the schema is visible in the CloudKit Dashboard and the container deletes the representative records.

Note

This method also validates the managed object model in use for a store, so if the model isn’t valid for use with CloudKit, a validation error may return.

## See Also

### Promoting Your Schema

struct NSPersistentCloudKitContainerSchemaInitializationOptions

Options that control the behavior when promoting the container’s schema to CloudKit.

