

- FSKit
-  FSManageableResourceMaintenanceOperations 

Protocol

# FSManageableResourceMaintenanceOperations

Maintenance operations for a file system’s resources.

macOS 15.4+

``` source
protocol FSManageableResourceMaintenanceOperations : NSObjectProtocol
```

## Overview

This protocol includes operations to check and format a resource for an FSUnaryFileSystem. Conform to this protocol if you implement a FSUnaryFileSystem that uses an FSBlockDeviceResource.

## Topics

### Checking the file system

func startCheck(task: FSTask, options: FSTaskOptions) throws -> Progress

Starts checking the file system with the given options.

**Required**

### Formatting the file system

func startFormat(task: FSTask, options: FSTaskOptions) throws -> Progress

Starts formatting the file system with the given options.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

