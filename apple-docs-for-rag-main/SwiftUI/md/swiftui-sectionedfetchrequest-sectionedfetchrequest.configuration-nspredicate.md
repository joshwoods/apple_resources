

- SwiftUI
- SectionedFetchRequest
- SectionedFetchRequest.Configuration
-  nsPredicate 

Instance Property

# nsPredicate

The request’s predicate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var nsPredicate: NSPredicate?
```

## Discussion

Set this configuration value to cause a SectionedFetchRequest to execute a fetch with a new predicate.

Access this value for a given request by using the nsPredicate property on the associated SectionedFetchResults instance, either directly or with a Binding.

