

- Device Management
-  declaration/asset/{identifier} 

Web Service Endpoint

# declaration/asset/{identifier}

The endpoint for fetching an asset declaration.

Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#declaration-asset-identifier
```

## Path Parameters

`identifier`

`string`

 (Required) 

The identifier of the asset declaration to fetch.

## Response Codes

` 200 ``OK`

DeclarationResponse

`OK`

The details of the asset declaration.

Content-Type: application/json

` 404 ``Not Found`

`Not Found`

The system doesn’t have an asset with the specified identifier.

## See Also

### Declaration Endpoints

declaration/activation/{identifier}

The endpoint for fetching an activation declaration.

declaration/configuration/{identifier}

The endpoint for fetching a configuration declaration.

declaration/management/{identifier}

The endpoint for fetching a management declaration.

