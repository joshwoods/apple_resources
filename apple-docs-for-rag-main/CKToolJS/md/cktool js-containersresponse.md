

- CKTool JS
-  ContainersResponse 

Structure

# ContainersResponse

An object that represents results of fetching multiple CloudKit containers.

CKTool JS 1.2.15+

``` source
dictionary ContainersResponse {
 string? nextKey;
 string? previousKey;
 Container[] containers;
 Container[]? recentContainers;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { ContainersResponse } from "@apple/cktool.database";
```

## Topics

### Instance Properties

containers

The list of containers.

nextKey

The record key for fetching the next page of results.

previousKey

The record key for fetching the previous page of results.

recentContainers

The list of recently accessed containers.

## See Also

### Global Structures and Enumerations

Container

Details about a CloudKit container.

CKEnvironment

An enumeration of container environments.

ContainersSortByField

An enumeration that indicates sorting options for retrieved containers.

SortDirection

An enumeration that indicates sorting direction when applying a custom sort.

