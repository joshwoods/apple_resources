

- Core Spotlight
- CSSearchableIndex
-  init(name:protectionClass:) 

Initializer

# init(name:protectionClass:)

Returns an on-device index with the specified name and data protection class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
init(
    name: String,
    protectionClass: FileProtectionType?
)
```

## Parameters 

`name`  

A name that pertains to your custom organization.

`protectionClass`  

The file protection class. Acceptable values are none, complete, completeUnlessOpen, or completeUntilFirstUserAuthentication.

## Return Value

An index that can handle items within the specified protection class.

## Mentioned in 

Adding your app’s content to Spotlight indexes

## Discussion

Use this method to specify a protection class for an index. You can specify a default protection class for index items in the entitlements for your app.

## See Also

### Creating an index

class func `default`() -> Self

Returns the default on-device index.

init(name: String)

Returns an on-device index with the specified name.

