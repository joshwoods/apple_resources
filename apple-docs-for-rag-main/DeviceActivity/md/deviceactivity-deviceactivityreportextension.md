

- DeviceActivity
-  DeviceActivityReportExtension 

Protocol

# DeviceActivityReportExtension

An app extension that reports device activity data.

DeviceActivitySwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
protocol DeviceActivityReportExtension : AppExtension
```

## Overview

Your extension is provided with the data that your app requests when it instantiates a `DeviceActivityReport`, which it uses to render a View representing the user’s device activity.

## Topics

### Associated Types

associatedtype Body : DeviceActivityReportScene

The body of the extension’s scene.

**Required**

### Instance Properties

var body: Self.Body

A body containing a DeviceActivityReportScene for each context that your extension supports.

**Required**

## Relationships

### Inherits From

- AppExtension

