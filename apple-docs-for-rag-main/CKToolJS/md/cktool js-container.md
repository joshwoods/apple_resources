

- CKTool JS
-  Container 

Structure

# Container

Details about a CloudKit container.

CKTool JS 1.2.15+

``` source
dictionary Container {
 string id;
 string teamId;
 string name;
 string? imageUrl;
 boolean? isHidden;
};
```

## Overview

Your app’s data is stored in a container. For information about what containers are available to you with CloudKit Console, see `https://icloud.developer.apple.com`. If you’re using Xcode, you can find your container identifier in your project’s Capability section.

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { Container } from "@apple/cktool.database";
```

## Topics

### Instance Properties

id

The unique identifier of the container.

imageUrl

The container’s image URL.

isHidden

Whether the container is hidden.

name

The container name.

teamId

The identifier of the developer team who owns the container.

## See Also

### Global Structures and Enumerations

ContainersResponse

An object that represents results of fetching multiple CloudKit containers.

CKEnvironment

An enumeration of container environments.

ContainersSortByField

An enumeration that indicates sorting options for retrieved containers.

SortDirection

An enumeration that indicates sorting direction when applying a custom sort.

