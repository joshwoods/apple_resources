

- Core Data
-  NSPersistentCloudKitContainerSchemaInitializationOptions 

Structure

# NSPersistentCloudKitContainerSchemaInitializationOptions

Options that control the behavior when promoting the container’s schema to CloudKit.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct NSPersistentCloudKitContainerSchemaInitializationOptions
```

## Topics

### Constants

static var dryRun: NSPersistentCloudKitContainerSchemaInitializationOptions

A flag that indicates the container validates the model and generates the records, but doesn’t upload them to CloudKit.

static var printSchema: NSPersistentCloudKitContainerSchemaInitializationOptions

Prints the generated records to the console.

### Initializers

init(rawValue: UInt)

Creates the schema initialization options using the specified raw value.

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

### Promoting Your Schema

func initializeCloudKitSchema(options: NSPersistentCloudKitContainerSchemaInitializationOptions) throws

Creates the CloudKit schema for all stores in the container that manage a CloudKit database.

