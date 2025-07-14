

- CKTool JS
-  CKToolNodeJsModule 

Class

# CKToolNodeJsModule

The imported package that supports using the client library within a Node.js environment.

CKTool JS 1.2.15+

``` source
interface CKToolNodeJsModule
```

## Overview

This is the import of all exported content from the `@apple/cktool.target.nodejs` package.

To configure the tool for Node.js import the `createConfiguration` function from the `@apple/cktool.target.nodejs` package.

```
import * as CKToolNodeJsModule from "@apple/cktool.target.nodejs";
// Example usage
const configuration = CKToolNodeJsModule.createConfiguration();
```

## Topics

### Instance Methods

createConfiguration

This function creates an instance of `Configuration` with suitable values for use in Node.js.

## See Also

### Configuration

Configuration

An object you use to hold options for communicating with the API server.

CKToolBrowserModule

The imported package that supports using the client library within a web browser.

