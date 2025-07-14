

- SwiftUI
- SectionedFetchRequest
- SectionedFetchRequest.Configuration
-  sectionIdentifier 

Instance Property

# sectionIdentifier

The request’s section identifier key path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var sectionIdentifier: KeyPath
```

## Discussion

Set this configuration value to cause a SectionedFetchRequest to execute a fetch with a new section identifier. You can’t change the section identifier type without creating a new fetch request. Use care to coordinate section and sort updates, as described in SectionedFetchRequest.Configuration.

Access this value for a given request by using the sectionIdentifier property on the associated SectionedFetchResults instance, either directly or with a Binding.

