

- RoomPlan
- CapturedRoom
-  CapturedRoom.ModelProvider 

Structure

# CapturedRoom.ModelProvider

A structure that assigns detailed 3D models to captured objects for an export.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct ModelProvider
```

## Overview

This structure provides a way for your app to assign detailed shape to specific areas within a captured room.

RoomPlan approximates the size and shape of objects it observes in a scan by using bounding boxes. In iOS 17 and later, the framework categorizes those objects that it recognizes by tagging them with specific attributes (Captured Object Attributes).

`ModelProvider` enables your app to export the categorized objects with unique 3D models. For example, you can assign a specific 3D model to a combination of attributes, such as all `.stool` objects with a `.star` base.

## Topics

### Creating a model provider

init()

Creates a model provider.

### Managing models

var modelFileURLs: [URL]

An array of URLs to 3D models for all categories and attributes.

func modelFileURL(for: CapturedRoom.Object.Category) throws -> URL?

Provides a URL to the 3D model for the given category.

func modelFileURL(for: CapturedRoom.Object) throws -> URL?

Provides a URL to a 3D model based on the given object’s attributes or category.

func modelFileURL(for: [any CapturedRoomAttribute]) throws -> URL?

Provides a URL to the 3D model for the given attributes.

func setModelFileURL(URL?, for: [any CapturedRoomAttribute]) throws

Associates a URL to the given attributes.

func setModelFileURL(URL?, for: CapturedRoom.Object.Category) throws

Associates a URL to the given object category.

### Handling errors

enum Error

Errors that can occur when managing 3D model association with categories and attributes.

## See Also

### Generating a USDZ file

func export(to: URL, exportOptions: CapturedRoom.USDExportOptions) throws

Produces a 3D asset from the captured room.

func export(to: URL, metadataURL: URL?, modelProvider: CapturedRoom.ModelProvider?, exportOptions: CapturedRoom.USDExportOptions) throws

Produces a 3D asset from the captured room with the given metadata output URL and model provider.

struct USDExportOptions

Options that determine the underlying data format of a scan export.

