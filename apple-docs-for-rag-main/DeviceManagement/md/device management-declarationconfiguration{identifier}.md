

- Device Management
-  declaration/configuration/{identifier} 

Web Service Endpoint

# declaration/configuration/{identifier}

The endpoint for fetching a configuration declaration.

Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#declaration-configuration-identifier
```

## Path Parameters

`identifier`

`string`

 (Required) 

The identifier of the configuration declaration to fetch.

## Response Codes

` 200 ``OK`

DeclarationResponse

`OK`

The details of the configuration declaration.

Content-Type: application/json

` 404 ``Not Found`

`Not Found`

The system doesn’t support the configuration declaration with the specified identifier.

## See Also

### Declaration Endpoints

declaration/activation/{identifier}

The endpoint for fetching an activation declaration.

declaration/asset/{identifier}

The endpoint for fetching an asset declaration.

declaration/management/{identifier}

The endpoint for fetching a management declaration.

