

- Device Management
- ParentalControlsApplicationRestrictions
-  ParentalControlsApplicationRestrictions.ApplicationItem 

Device Management Profile

# ParentalControlsApplicationRestrictions.ApplicationItem

A dictionary defining an app for parental control.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ParentalControlsApplicationRestrictions.ApplicationItem
```

## Properties

`appID`

`data`

 (Required) 

The identifier of the app. Obtain this value from the Security framework using SecCodeCopyDesignatedRequirement(_:_:_:).

`bundleID`

`string`

 (Required) 

The bundle ID of the app.

`detachedSignature`

`data`

The signature for an unsigned binary.

`disabled`

`boolean`

If `true`, this app isn’t added to the allow list.

Default: `false`

`displayName`

`string`

The name used for display purposes.

`subApps`

`[`ParentalControlsApplicationRestrictions.ApplicationItem`]`

An array of nested helper applications.

