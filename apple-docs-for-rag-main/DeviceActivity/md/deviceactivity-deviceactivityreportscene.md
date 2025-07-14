

- DeviceActivity
-  DeviceActivityReportScene 

Protocol

# DeviceActivityReportScene

Defines a custom device activity report scene.

DeviceActivitySwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
protocol DeviceActivityReportScene : AppExtensionScene
```

## Overview

This protocol refines `AppExtensionScene` and restricts the types that can be passed to a DeviceActivityReportBuilder. Your extension should provide a scene for each context that your app supports.

## Topics

### Associated Types

associatedtype Configuration

A type used to configure your scene’s content.

**Required**

associatedtype Content : View

The type of view that represents the scene’s content.

**Required**

### Instance Properties

var content: (Self.Configuration) -> Self.Content

A closure that builds your report’s content with the provided configuration.

**Required**

var context: DeviceActivityReport.Context

The context of the scene.

**Required**

### Instance Methods

func makeConfiguration(representing: DeviceActivityResults&lt;DeviceActivityData>) async -> Self.Configuration

Creates a new configuration that represents the provided data.

**Required**

## Relationships

### Inherits From

- AppExtensionScene

