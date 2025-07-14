

- Device Management
-  StatusAccountListLDAP 

Object

# StatusAccountListLDAP

A status report of the client’s LDAP accounts.

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object StatusAccountListLDAP
```

## Properties

`account.list.ldap`

`[`StatusAccountListLDAPAccountObject`]`

 (Required) 

A list of status values for the LDAP accounts.

## Topics

### Supporting Objects

object StatusAccountListLDAPAccountObject

A status report of the client’s LDAP account details.

## See Also

### Status Account List Elements

object StatusAccountListCalDAV

A status report of the client’s CalDAV accounts.

object StatusAccountListCardDAV

A status report of the client’s CardDAV accounts.

object StatusAccountListExchange

A status report of the client’s exchange accounts.

object StatusAccountListGoogle

A status report of the client’s Google accounts.

object StatusAccountListMailIncoming

A status report of the client’s incoming mail accounts.

object StatusAccountListMailOutgoing

A status report of the client’s outgoing mail accounts.

object StatusAccountListSubscribedCalendar

A status report of the client’s calendar accounts.

