

- CKTool JS
- PromisesApi
-  validateSchema 

Instance Method

# validateSchema

Validates the uploaded schema file for the container.

CKTool JS 1.2.15+

``` source
CancellablePromise validateSchema(
 ValidateSchemaParams params
);
```

## Parameters 

`params`  

A dictionary as described in the Discussion section.

## Return Value

A `CancellablePromise` with the following resolutions.

## Discussion

If the promise is successful, it will resolve with one of the following dictionaries:

- `{ statusCode: 200; result: CKDBValidateSchemaResponse }`

The promise may reject and throw the following:

- `DocumentedResponseError`, if the HTTP status code is 421. The result member will be a dictionary conforming to AuthenticationRequiredError.

- `DocumentedResponseError`, if the HTTP status code is none of the above and in the range 400 to 599. The result member will be a dictionary conforming to RequestError.

- `ValidationError`, if the parameters to the method are incorrect.

- A `FetchError` descendant, if there is a problem with the network request. A reference to the request object can be used to examine the underlying cause.

## Discussion

The `params` dictionary has the following properties:

```
dictionary ValidateSchemaParams {
  File file;
  string teamId;
  string containerId;
  CKEnvironment environment;
}
```

- `file`:

- `teamId`: The team identifier. You can find your team identifier in the Membership tab of the Apple Developer portal at `https://developer.apple.com`.

- `containerId`: The container identifier. See `Container`.

- `environment`: The container environment. For valid values, see `CKEnvironment`.

If the operation completes successfully, the response contains a result with a `CKDBValidateSchemaResponse` object. A schema validates successfully only if it has the correct syntax and if `importSchema` is able to import it successfully to the container. The text you provide in the file object must be in CloudKit Schema Language. To learn more about CloudKit Schema Language, see `https://developer.apple.com/documentation/cloudkit/integrating_a_text-based_schema_into_your_workflow`. Related: `exportSchema`, `importSchema`.

Node.js example:

```

import { CKEnvironment, PromisesApi } from "@apple/cktool.database";
import { File, createConfiguration } from "@apple/cktool.target.nodejs";
import fs from "fs/promises";
import path from "path";

try {
  const api = new PromisesApi({
    configuration: createConfiguration(),
    security: {
      // You can obtain a management token from the
      // Database section of CloudKit Console.
      "ManagementTokenAuth": "YOUR_MANAGEMENT_TOKEN"
    },
  });

  console.log(`Validating schema...`);
  // Read a schema file from the file system
  const srcPath = path.join(__dirname, "sample.CKDB");
  const buffer = await fs.readFile(srcPath);
  // Wrap in a File object.
  const file = new File([buffer], "sample.CKDB");
  const { result } = await api.validateSchema({
    teamId: "YOUR_TEAM_ID",
    containerId: "YOUR_CONTAINER_ID",
    environment: CKEnvironment.DEVELOPMENT,
    file,
  });
  if (result.isValid) {
    console.log(`Schema validated successfully`);
  } else {
    console.log(`Schema did not pass validation`);
  }
} catch(ex) {
  // Handle error
}
```

## See Also

### Database Management

exportSchema

Downloads the container’s schema.

getContainers

Fetches containers for a team.

importSchema

Uploads a file that defines the new schema for the container.

resetConfigToProduction

Resets the container configuration to production.

resetToProduction

Resets the schema of the environment to production.

