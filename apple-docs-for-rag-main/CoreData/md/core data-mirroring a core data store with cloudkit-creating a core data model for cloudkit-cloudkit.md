

- Core Data
- Mirroring a Core Data store with CloudKit
-  Creating a Core Data Model for CloudKit 

Article

# Creating a Core Data Model for CloudKit

Design a CloudKit-compatible data model and initialize your CloudKit schema.

## Overview

To pass records between a Core Data store and a CloudKit database, they both require a shared understanding of the data structure. You define this in the Core Data model and then use that to generate a CloudKit schema.

### Create a Data Model

Use Xcode’s Core Data model editor to define your app’s entities and their attributes, or construct your model in code. For more information, see Creating a Core Data model and the articles under Modeling data.

CloudKit doesn’t support all the features of a Core Data model. As you design your model, be aware of the following limitations and make sure you create a compatible data model.

| Core Data model element | CloudKit schema limitation |
|----|----|
| **Entities** | Unique constraints aren’t supported. |
| **Attributes** | `Undefined` and objectID attribute types aren’t supported. |
| **Relationships** | All relationships must be optional. Due to operation size limitations, CloudKit may not save relationship changes atomically.  All relationships must have an inverse, in case the records synchronize out of order.  CloudKit doesn’t support the Deny deletion rule. |
| **Configurations** | Entities in a configuration must not have relationships to entities in another configuration. |

For more information about how Core Data translates managed objects to CloudKit records, see Reading CloudKit Records for Core Data.

### Initialize Your CloudKit Schema During Development

After creating your Core Data model, inform CloudKit about the types of records it contains by initializing a development schema. This is a draft schema that you can rewrite as often as necessary during development. You can’t delete a record type or modify any existing attributes after you promote a development schema to production.

Use the persistent container to initialize the development schema, which you can do during app launch or from within one or more integration tests. To exclude schema initialization from your production builds, use the following:

```
let container = NSPersistentCloudKitContainer(name: "Earthquakes")

// Only initialize the schema when building the app with the 
// Debug build configuration.        
#if DEBUG
do {
    // Use the container to initialize the development schema.
    try container.initializeCloudKitSchema(options: [])
} catch {
    // Handle any errors.
}
#endif
```

After initializing the schema, the console contains an entry similar to the following:

```
: Successfully set up CloudKit 
    integration for store
```

While initializing the schema, Core Data creates a temporary instance of each distinct record type in each of the container’s stores that mirror to a CloudKit database and uploads them to the iCloud servers. After completing the upload, the schema is visible in the CloudKit dashboard and Core Data removes the temporary records.

For more information about configuring a CloudKit persistent container, see Setting Up Core Data with CloudKit.

### Reset the Environment

As you change the model during development, periodically visit the CloudKit dashboard to reset the development environment and delete the existing development schema, before initializing a new one. For more information about resetting the development environment, see Using CloudKit Dashboard to Manage Databases.

### Promote the Schema to Production

When you’re happy with your data model, have a fully tested app, and are ready to submit it to the App Store, it’s time to promote your schema from development to production.

Important

After you promote your schema to production, the record types and their fields are immutable and exist for all time. You can add new record types, and additional fields to existing record types, but you can’t modify or delete existing record types.

Initialize your schema one last time, then promote it from the CloudKit dashboard. For more information about promoting a schema from development to production, see Deploying the Schema.

### Update the Production Schema

Plan carefully for how your app handles forward compatibility and major changes to the data model, because you can’t rename or delete CloudKit record types and fields in production. Consider these strategies:

- Migrate users to a completely new store, using NSPersistentCloudKitContainerOptions to associate the new store with a new container.

- Incrementally add new fields to existing record types. If you adopt this approach, older versions of your app have access to every record a user creates, but not every field.

- Version your entities by including a `version` attribute from the outset, and use a fetch request to select only those records that are compatible with the current version of the app. If you adopt this approach, older versions of your app won’t fetch records that a user creates with a more recent version, effectively hiding them on that device.

For example, consider a `Post` entity with a `version` attribute that stores the version of the app that creates the record. You can use a predicate to fetch only the records that are compatible with the current version of the app.

```
// The current version of the app's data model.
let maxCompatibleVersion = 3

let context = NSManagedObjectContext(
    concurrencyType: .privateQueueConcurrencyType
)

context.performAndWait {
    let fetchRequest = NSFetchRequest(entityName: "Post")

    // Create a predicate that matches against the version attribute.
    fetchRequest.predicate = NSPredicate(
        format: "version 

Along with these choices, consider your timelines for supporting multiple versions of your app, and for migrating users to newer app versions.

For tips on migrating records to a new schema, see Designing for CloudKit. For more information about Core Data model migration, see Migrating your data model automatically. For heavyweight migrations, see the Core Data Model Versioning and Data Migration guide.

## See Also

### Configuring CloudKit Mirroring

Setting Up Core Data with CloudKit

Set up the classes and capabilities that sync your store to CloudKit.

Syncing a Core Data Store with CloudKit

Synchronize objects between devices, and handle store changes in the user interface.

Reading CloudKit Records for Core Data

Access CloudKit records created from Core Data managed objects.

