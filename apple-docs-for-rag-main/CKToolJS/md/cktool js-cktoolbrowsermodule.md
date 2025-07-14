

- CKTool JS
-  CKToolBrowserModule 

Class

# CKToolBrowserModule

The imported package that supports using the client library within a web browser.

CKTool JS 1.2.15+

``` source
interface CKToolBrowserModule
```

## Overview

This is the import of all exported content from the `@apple/cktool.target.browser` package.

To configure the tool for web browsers import the `createConfiguration` function from the `@apple/cktool.target.browser` package.

```
import * as CKToolBrowserModule from "@apple/cktool.target.browser";
// Example usage
const configuration = CKToolBrowserModule.createConfiguration();
```

## Topics

### Instance Methods

createConfiguration

This function creates an instance of `Configuration` with suitable values for use in web browsers.

## See Also

### Configuration

Configuration

An object you use to hold options for communicating with the API server.

CKToolNodeJsModule

The imported package that supports using the client library within a Node.js environment.

