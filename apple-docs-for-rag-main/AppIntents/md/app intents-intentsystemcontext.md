

- App Intents
-  IntentSystemContext 

Structure

# IntentSystemContext

Information that the system makes available to an app intent while it performs its action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentSystemContext
```

## Overview

Access information the system provides to your app intent while it performs its action in its perform() implementation. The provided information can vary and include information for each platform. For example, in watchOS, the intent system context includes a precise timestamp when a person started the app intent’s action using the Action button on Apple Watch Ultra.

## Topics

### Instance Properties

var preciseTimestamp: Date?

A precise timestamp for the performed action.

## See Also

### Supplementary content

protocol AppIntentsPackage

A type that describes app intent definitions that aren’t part of an app bundle and their dependencies.

struct IntentDescription

The human-readable description and metadata for an app intent.

struct IntentDialog

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

struct IntentDeprecation

class IntentProjection

Projections for an app intent that returns non-optional values for parameters.

