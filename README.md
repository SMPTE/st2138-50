# ST 2138-50

## General

_This repository is *public*._

Please consult [CONTRIBUTING.md](./CONTRIBUTING.md), [CONFIDENTIALITY.md](./CONFIDENTIALITY.md), [LICENSE.md](./LICENSE.md) and
[PATENTS.md](./PATENTS.md) for important notices.

Your feedback is welcome at _link to GitHub issue tracker_ or at _TC chair email address_.

## Public Committee Draft (PCD) Notice

The following elements are made available for a public review period ending no earlier than {YYYY-MM-DD}, and no later than {YYYY-MM-DD}:

* [{prose element}]({link to prose element})
* [{element #1}]({link to element #1})
* ...

## Details
Security, when it comes to control of media devices, is no longer a “nice to have”. It is a requirement.

This document is focused on how to securely use the control protocol specified in ST 2138-10 with respect to authenticity, integrity, access control, confidentiality and availability.

This document is applicable to how the following are to be supported by compliant devices and services:

* Authenticity
  * Clients can verify that communications are from the device and no other source.
  * Devices can verify that the access tokens accompanying each request were issued by the authorization server in the token’s iss claim.
* Integrity — Clients can trust that communications from a compliant device or service have not been tampered with in transit.
* Which OAuth2 Access Control flows are used by clients and supported by a compliant device or service.
* Access Control
  * The responsibility of the device to provide Policy Enforcement Point functionality, and how this responsibility may optionally be divided between devices and gateways.
  * Access revocation functionality required by the device.
  * Correct handling in the event of access token expiry.
* Confidentiality — Confidentiality of data in transit.
* Availability — How timely access to device capabilities is promoted by using JWS rather than opaque access tokens, thereby avoiding round trips by devices to the Authorization server’s introspection endpoint.
