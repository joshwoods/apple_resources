

- CloudKit
- CKContainer
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a container for the specified identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
init(identifier containerIdentifier: String)
```

## Parameters 

`containerIdentifier`  

The bundle identifier of the app with the container that you want to access. The bundle identifier must be in the app’s `com.apple.developer.icloud-container-identifiers` entitlement. This parameter must not be `nil`.

## Discussion

The specified identifier must correspond to one of the ubiquity containers in the iCloud capabilities section of your Xcode project. Including the identifier with your app’s capabilities adds the corresponding entitlements to your app. To access your app’s default container, use the default() method instead.

## See Also

### Creating Containers

class func `default`() -> CKContainer

Returns the app’s default container.

