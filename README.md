# Itemora Books — compliance rules

This repository holds one file, `latest.json`: the current signed rules pack for
Itemora Books. It contains Australian tax, superannuation, leave and public-holiday
figures taken from Australian Taxation Office and Fair Work Ombudsman publications,
and a signature. It contains nothing about any business.

Itemora Books downloads this file when a user chooses *Check for updates*, and
installs it only if the signature matches the publisher key built into the
application and the version is newer than the one in use.

The figures are provided for use by Itemora Books. They are not tax advice; check
the ATO and Fair Work Ombudsman for the authoritative position.

Do not edit `latest.json` by hand — an edited file fails its signature and is
refused. It is published from the Itemora Books source with
`npm run rules:publish`.
