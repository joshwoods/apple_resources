

- SwiftUI
- FetchRequest
- FetchRequest.Configuration
-  nsPredicate 

Instance Property

# nsPredicate

The request’s predicate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
var nsPredicate: NSPredicate?
```

## Discussion

Set this configuration value to cause a FetchRequest to execute a fetch with a new predicate.

Access this value of a FetchRequest.Configuration structure for a given request by using the nsPredicate property on the associated FetchedResults instance, either directly or through a Binding.

