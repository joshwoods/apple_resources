

- App Intents
-  Common types 

API Collection

# Common types

Specify common types that your app supports, including currencies, files, and contacts.

## Overview

Use these types to manage specific types of data when you create a parameter for an app intent or a property for an app entity.

## Topics

### Contacts

struct IntentPerson

Information that identifies a person participating in an intents-based interaction.

### Files

struct IntentFile

An interface for providing an app entity that represents an on-disk file or file-based resource.

### Monetary types

struct IntentCurrencyAmount

An amount of money to transfer during a financial transaction.

struct IntentPaymentMethod

Information about a form of payment supported by your app.

### Items and collections

struct IntentItem

A type describing a value returned from a dynamic options provider, plus information about how to display it to users.

struct IntentItemCollection

Return this object to provide an advanced list of options, optionally divided in sections.

struct IntentItemSection

An object you use to divide dynamic options into sections.

struct IntentCollectionSize

