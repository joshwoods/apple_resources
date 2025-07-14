

- CKTool JS
-  CancellablePromise 

Class

# CancellablePromise

A promise that has a function to cancel its operation.

CKTool JS 1.2.15+

``` source
interface CancellablePromise
```

## Overview

This class wraps an ordinary promise, but also provides a method that can be used to cancel the promise. The `cancel` function throws `CancelledError` if called.

API object methods return a promise of this type. For example, `PromisesApi` has a `createRecord` method that returns a `CancellablePromise`.

## Topics

### Initializers

CancellablePromise

### Instance Properties

inner

The wrapped promise.

### Instance Methods

cancel

Stops any work the promise is doing.

catch

Tells `CancellablePromise` what callback to call on failure of the inner promise.

finally

Tells `CancellablePromise` what callback to call when the inner promise either succeeds or fails.

then

Tells `CancellablePromise` what callbacks to call on success or failure of the inner promise.

## See Also

### Promises API

PromisesApi

A class that exposes promise-based functions for interacting with the API.

CKToolDatabaseModule

The imported package that provides access to CloudKit containers and databases.

