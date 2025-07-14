

- Core Data
- NSLightweightMigrationStage
-  init(\_:) 

Initializer

# init(\_:)

Creates a lightweight migration stage with the specified version checksums.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+Swift 5.8+

``` source
convenience init(_ checksums: [String])
```

## Parameters 

`checksums`  

The array of version checksums.

## Discussion

To determine an object model’s version checksum, use its versionChecksum property. Alternatively, you can find the checksum in the versioned model’s `VersionInfo.plist` file or in Xcode’s build log.

