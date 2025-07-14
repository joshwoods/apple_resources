

- CKTool JS
-  CKToolDatabaseModule 

Class

# CKToolDatabaseModule

The imported package that provides access to CloudKit containers and databases.

CKTool JS 1.2.15+

``` source
interface CKToolDatabaseModule
```

## Overview

This is the import of all exported content from the `@apple/cktool.database` package.

To access members of `CKToolDatabaseModule` import the `@apple/cktool.database` package the following way:

```
import * as CKToolDatabaseModule from "@apple/cktool.database";
// Example usage
const result = CKToolDatabaseModule.toByte(123);
```

Alternatively, you can import the package symbols directly:

```
import { toByte } from "@apple/cktool.database";
// Example usage
const result = toByte(123);
```

Importing package symbols this way supports tree-shaking.

## Topics

### Instance Methods

createUuid

Creates a new `Uuid`.

toBase64String

Converts a regular string to a `Base64String`.

toByte

Converts a numeric value to a `Byte`.

toByteArray

Converts a numeric array to a `ByteArray`.

toDouble

Converts a number or numeric string to a `Double`.

toFloat

Converts a number or numeric string to a `Float`.

toInt32

Converts a number to an `Int32`.

toInt64

Converts a number or numeric string to a `Int64`.

toNumber

Converts a supported numeric type to a JavaScript number.

toUuid

Converts a string to a `Uuid`.

## See Also

### Promises API

PromisesApi

A class that exposes promise-based functions for interacting with the API.

CancellablePromise

A promise that has a function to cancel its operation.

