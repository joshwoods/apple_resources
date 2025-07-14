

- CloudKit
- CKContainer
-  default() 

Type Method

# default()

Returns the app’s default container.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class func `default`() -> CKContainer
```

## Mentioned in 

Designing and Creating a CloudKit Database

## Discussion

Use this method to retrieve your app’s default container. This is the one you typically use to store your app’s data. If you want the container for a different app, create a container using the init(identifier:) method.

During development, the container uses the development environment. When you release your app, the container uses the production environment.

## See Also

### Creating Containers

init(identifier: String)

Creates a container for the specified identifier.

