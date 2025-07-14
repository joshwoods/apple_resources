

- Contacts UI
- ContactAccessButton
-  ContactAccessButton.Caption 

Enumeration

# ContactAccessButton.Caption

A list of access options to display in the contact access button when matching a contact’s name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
enum Caption
```

## Overview

Set the caption of a contact access button with the view modifier contactAccessButtonCaption(_:). When the query produces a single result, the content access button shows the the caption under the matching contact name. For example, a search for `Anne` could show a button that displays the matching name “Anne Johnson” with a caption line of “annejohnson1@icloud.com” when the caption type is ContactAccessButton.Caption.email.

## Topics

### Caption options

case defaultText

A caption option that displays a default value.

case email

A caption option that displays an email address for the contact.

case phone

A caption option that displays a phone number for the contact.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

