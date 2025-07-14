

- SwiftUI
- SectionedFetchRequest
-  SectionedFetchRequest.Configuration 

Structure

# SectionedFetchRequest.Configuration

The request’s configurable properties.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Configuration
```

## Overview

You initialize a SectionedFetchRequest with a section identifier, an optional predicate, and sort descriptors, either explicitly or with a configured NSFetchRequest. Later, you can dynamically update the identifier, predicate, and sort parameters using the request’s configuration structure.

You access or bind to a request’s configuration components through properties on the associated SectionedFetchResults instance, just like you do for a FetchRequest using FetchRequest.Configuration.

When configuring a sectioned fetch request, ensure that the combination of the section identifier and the primary sort descriptor doesn’t create discontiguous sections.

## Topics

### Setting the section identifier

var sectionIdentifier: KeyPath&lt;Result, SectionIdentifier>

The request’s section identifier key path.

### Setting a predicate

var nsPredicate: NSPredicate?

The request’s predicate.

### Setting sort descriptors

var sortDescriptors: [SortDescriptor&lt;Result>]

The request’s sort descriptors, accessed as value types.

var nsSortDescriptors: [NSSortDescriptor]

The request’s sort descriptors, accessed as reference types.

## See Also

### Configuring a request dynamically

var projectedValue: Binding&lt;SectionedFetchRequest&lt;SectionIdentifier, Result>.Configuration>

A binding to the request’s mutable configuration properties.

