

- Device Management
-  declaration/activation/{identifier} 

Web Service Endpoint

# declaration/activation/{identifier}

The endpoint for fetching an activation declaration.

Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#declaration-activation-identifier
```

## Path Parameters

`identifier`

`string`

 (Required) 

The identifier of the activation declaration to fetch.

## Response Codes

` 200 ``OK`

DeclarationResponse

`OK`

The details of the activation declaration.

Content-Type: application/json

` 404 ``Not Found`

`Not Found`

The system doesn’t support the activation declaration with the specified identifier.

## See Also

### Declaration Endpoints

declaration/asset/{identifier}

The endpoint for fetching an asset declaration.

declaration/configuration/{identifier}

The endpoint for fetching a configuration declaration.

declaration/management/{identifier}

The endpoint for fetching a management declaration.

