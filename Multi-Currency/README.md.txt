# Salesforce CPQ - Multi Currency

## Scenario

Created a product named **1 gm Gold Ring**.

Created Price Book Entries in:
- INR
- USD

Created a Quote.

## Problem

The product was not appearing in the Quote Line Editor when the Price Book Entry currency was USD.

## Root Cause

The Quote Currency was INR, while the Product Price Book Entry Currency was USD.

Salesforce CPQ only displays products whose Price Book Entry currency matches the Quote currency.

## Solution

Changed the Quote Currency from INR to USD.

## Result

The product appeared successfully in the Quote Line Editor.

## Key Learning

- One Quote supports only one currency.
- One Quote supports only one Price Book.
- Products are filtered based on the Quote Currency.
- Quote Currency must match the Price Book Entry Currency.