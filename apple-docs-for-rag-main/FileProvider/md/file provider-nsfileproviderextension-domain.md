

- File Provider
- NSFileProviderExtension
-  domain 

Instance Property

# domain

The domain managed by this file provider object.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
var domain: NSFileProviderDomain? { get }
```

## Discussion

If the File Provider extension does not use domains, this property is set to `nil`. By default, a File Provider extension does not have any domains.

A new NSFileProviderExtension object is created for each domain added to the File Provider manager. The new File Provider’s domain property is set to the added domain, and any items returned by the File Provider belong to that domain.

