

- App Intents
-  IntentProjection 

Class

# IntentProjection

Projections for an app intent that returns non-optional values for parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@dynamicMemberLookup
final class IntentProjection where Intent : AppIntent
```

## Overview

Use an `IntentProjection` to create an app intent that returns non-optional values for parameters you list using an IntentParameterDependency property wrapper.

## Topics

### Subscripts

subscript&lt;Value>(dynamicMember _: KeyPath&lt;Intent, Value>) -> Value.UnwrappedType

## See Also

### Supplementary content

protocol AppIntentsPackage

A type that describes app intent definitions that aren’t part of an app bundle and their dependencies.

struct IntentDescription

The human-readable description and metadata for an app intent.

struct IntentDialog

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

struct IntentDeprecation

struct IntentSystemContext

Information that the system makes available to an app intent while it performs its action.

