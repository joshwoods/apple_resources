

- CKTool JS
- PromisesApi
-  PromisesApi 

Initializer

# PromisesApi

Creates a `PromisesApi` object.

CKTool JS 1.2.15+

``` source
new defaultOptions(
 PromisesApiOptions defaultOptions
);
```

## Parameters 

`defaultOptions`  

A dictionary as described in the Discussion section.

## Discussion

You create an instance of `PromisesApi` in order to interact with the API. Methods on this class return promises that complete with a response object.

```
import { PromisesApi } from "@apple/cktool.database";
import { createConfiguration } from "@apple/cktool.target.nodejs";

const api = new PromisesApi({
  configuration: createConfiguration(),
  security: { “ManagementTokenAuth”: “YOUR_MANAGEMENT_TOKEN” }
});
```

The `defaultOptions` dictionary has the following properties:

```
dictionary PromisesApiOptions {
  Configuration: configuration;
  Security?: security;
}
```

- `configuration`: The `Configuration` instance created with `createConfiguration`.

- `security`: The dictionary of your authorization tokens.

## See Also

### Initialization

PromisesApiOptions

A dictionary of options for promises API classes.

Security

A dictionary of your authorization tokens.

