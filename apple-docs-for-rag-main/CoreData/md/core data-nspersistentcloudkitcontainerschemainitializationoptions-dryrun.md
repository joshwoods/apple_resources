

- Core Data
- NSPersistentCloudKitContainerSchemaInitializationOptions
-  dryRun 

Type Property

# dryRun

A flag that indicates the container validates the model and generates the records, but doesn’t upload them to CloudKit.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var dryRun: NSPersistentCloudKitContainerSchemaInitializationOptions { get }
```

## Discussion

This option is useful for unit testing to ensure your managed object model is valid for use with CloudKit.

## See Also

### Constants

static var printSchema: NSPersistentCloudKitContainerSchemaInitializationOptions

Prints the generated records to the console.

