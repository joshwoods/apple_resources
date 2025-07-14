

- Device Management
-  declaration/management/{identifier} 

Web Service Endpoint

# declaration/management/{identifier}

The endpoint for fetching a management declaration.

Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#declaration-management-identifier
```

## Path Parameters

`identifier`

`string`

 (Required) 

The identifier of the management declaration to fetch.

## Response Codes

` 200 ``OK`

DeclarationResponse

`OK`

The details of the management declaration.

Content-Type: application/json

` 404 ``Not Found`

`Not Found`

The system doesn’t support the management declaration with the specified identifier.

## See Also

### Declaration Endpoints

declaration/activation/{identifier}

The endpoint for fetching an activation declaration.

declaration/asset/{identifier}

The endpoint for fetching an asset declaration.

declaration/configuration/{identifier}

The endpoint for fetching a configuration declaration.

