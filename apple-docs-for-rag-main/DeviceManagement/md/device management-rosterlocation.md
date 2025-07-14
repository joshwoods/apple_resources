

- Device Management
-  RosterLocation 

Object

# RosterLocation

A location’s properties and their values.

Device Assignment ServicesVPP License Management

``` source
object RosterLocation
```

## Properties

`name`

`string`

The location name. Maximum length 1024 UTF-8 characters.

`op_date`

`string`

The time stamp, in iSO 8601 format, when the location was added, updated, or deleted.

`source`

`string`

The data source where the location was created.

Possible Values: `LDAP, SIS, CSV, MANUAL, SYSTEM, ENROLLMENT, DEP, FORMULA_GENERATED, SFTP`

`source_system_identifier`

`string`

The identifier configured by organization for the location. Maximum length 256 UTF-8 characters.

`status`

`string`

The status of the location.

`unique_identifier`

`string`

The unique identifier for the location. Maximum length 256 UTF-8 characters.

## See Also

### Location Mangement

object BaseRosterLocation

A base location’s properties and their values.

Get the List of Locations

Obtain a list of the locations the server manages.

Sync the Locations

Get updates about the list of locations the server manages.

