

- CKTool JS
-  CKEnvironment 

Enumeration

# CKEnvironment

An enumeration of container environments.

CKTool JS 1.2.15+

``` source
interface CKEnvironment {
 const string DEVELOPMENT;
 const string PRODUCTION;
};
```

## Overview

During initial development of your app, you create your schema and add records for testing in the development environment. Apps sold in the App Store can only access the production environment. Before you publish your app, you must deploy the development schema to the production environment to copy over its record types, fields, and indexes.

```
```

## Topics

### Enumeration Cases

DEVELOPMENT

PRODUCTION

## See Also

### Global Structures and Enumerations

Container

Details about a CloudKit container.

ContainersResponse

An object that represents results of fetching multiple CloudKit containers.

ContainersSortByField

An enumeration that indicates sorting options for retrieved containers.

SortDirection

An enumeration that indicates sorting direction when applying a custom sort.

