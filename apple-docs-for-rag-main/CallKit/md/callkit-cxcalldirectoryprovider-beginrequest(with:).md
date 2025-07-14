

- CallKit
- CXCallDirectoryProvider
-  beginRequest(with:) 

Instance Method

# beginRequest(with:)

Tells the extension to prepare for a host app’s request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
func beginRequest(with context: CXCallDirectoryExtensionContext)
```

## Parameters 

`context`  

A `CXCallDirectoryExtensionContext` object that represents the context in which the host app makes the request.

## Mentioned in 

Identifying and blocking calls

## Discussion

An extension prepares for a host app’s request by getting the context passed in this method and requesting related data items, if appropriate. This method is received after the extension is initialized, but before the principal object is asked to do anything with the context.

