## 1.2.0

> Released: 2021-11-04

> [Release Plan](https://github.com/shareportation/governance/wiki/Release-1.2.0)

The 1.2.0 minor release adds digital program Requirements, new options for policies, better GPS telemetry data, and moves Provider Vehicles out of beta. 

### CHANGES

See the closed PRs tagged with [Milestone 1.2.0](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pulls?q=is%3Apr+is%3Aclosed+milestone%3A1.2.0) and [Issues](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues?q=is%3Aissue+milestone%3A1.2.0+is%3Aclosed) for a full list of changes.

**_General SPP_**

- [Richer telemetry data](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/589), including [616](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/616), [73](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/73), [51](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/51)
- [Add cargo_bicycle vehicle type](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/698)

**_Policy_**

- [Program Requirements](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/646) - For agencies to describe program requirements digitally to allow providers and the public to see what SPP and GBFS versions, APIs, endpoints, and fields are required, and communicate available SPP agency information to providers.
  - [Ability to express data sharing requirements in Policy](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/608) 
  - [Method to Exclude some Provider Fields from Response](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/507)
  - [Retrieve operational zones from operators](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/639)
  - [Make Trip 'route' field optional for privacy](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/504)

- [Multiple options added to Policy](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/658)
   - [Add rate options to other rules types](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/633)
   - [Support parking fees by duration](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/631)
   - [Min and max clarity on Rules](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/689)
   - [Add a "rate applies when" field to Rules](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/666)

**_Provider_**

- [Vehicles out of beta](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/637)
- [Clarify use cases between SPP Vehicles and GBFS](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/641)

_Minor Updates_

- [Clarify single object response on policy/geography](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/599)
- [Schema updates](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/693), including [645](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/645), [687](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/687), [683](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/683)
- Add VeoRide, Boaz Bikes, and update Superpedestrian provider IDs

## 1.1.1

> Released: 2021-09-24 

The 1.1.1 support release fixes the version validation for 1.1.0 in the JSON schema, and adds comms_restored to removed state. 

### CHANGES

- ["removed" missing "comms_restored" option in provider schemas](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/690)
- [Version number is 1.0.x for 1.1.0 release](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/669)

## 1.1.0

> Released: 2021-03-30 

> [Release Plan](https://github.com/shareportation/governance/wiki/Release-1.1.0)

The 1.1.0 minor release adds new top level APIs (geography, jurisdictions), privacy options (provider reports, geography-driven events, metrics), and transparency features (public endpoints). 

### CHANGES

See the closed PRs tagged with [Milestone 1.1.0](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pulls?q=is%3Apr+is%3Aclosed+milestone%3A1.1.0) and [Issues](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues?q=is%3Aissue+milestone%3A1.1.0+is%3Aclosed) for a full list of changes.

**_SPP_**

- [Policy and Geography can be public](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/585)
- [Geography-Driven Events](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/503): [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/480)
   
_Minor Updates_

- [Unregistered error](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/565)
- [Geography updates](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/474)
- [Stops updates](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/603)
- [Response time expectations](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/563)
- [Geography publish date field consistency](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/597)
- [Adding more cities using SPP](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/591)
- [Adding more providers using SPP](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/blob/dev/providers.csv)
- [Added a section for third party software companies using SPP](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/552) and cleaned up home page, moving list content to the SPP website
- [Update geography_json field type](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/635)

**_Provider_**

- [New Reports](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/607): [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/569)

**_Agency_**

- N/A

**_Policy_**

- [Images of Stops](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/555)
- [Clarify update frequency](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/609): [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/567)

**_Geography_**

- [Elevating Geography to a first class API](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/582): [PR](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/499), [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/500)
- [Geography Types](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/581): [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/580), [Discussion](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/discussions/588)

**_Metrics_**

- [New Agency Metrics API](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/485): [Definitions PR](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/487), [Spec PR](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/486), [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/485)

**_Jurisdiction_**

- [New Jurisdiction API](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/593): [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/474)

## 1.0.0

> Released: 2020-09-16

> [Release Plan](https://github.com/shareportation/governance/wiki/Release-1.0.0)

The 1.0.0 release reconciles and aligns many parts of the SPP specification and adds features and updates requested by the community, including many new detailed vehicle states and event types, support for Stops (for docked vehicles, dockless corrals, parking areas), and adding rates (fees/subsidies) to Policy.

### CHANGES

See the closed PRs tagged with [Milestone 1.0.0](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pulls?q=is%3Apr+is%3Aclosed+milestone%3A1.0.0) for a full list of changes.

*_SPP_*

* [Reconcile the Provider and Agency language differences](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/506)
  * [New State Machine Diagram](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/530)
  * [JSON Schema updates](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/534)
  * [Add 'located' event_type](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/570)
  * [Update Unknown/Unspecified transitions](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/558)
  * [Add 'unspecified' events where needed](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/560)
* [Adding Stops](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/427) - Beta
   
* Minor Updates 
  * [Update cities using SPP](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/520)
  * Update [Austin](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/488), [Louisville](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/515) links
  * [Add link to State of Practice](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/477)
  * [Update GBFS references and links](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/508)
  * Move [Code of Conduct](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/514), [Contributing Guide](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/513), and [Release Guidelines](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/512) to new [Governance repo](https://github.com/shareportation/governance)
   * [Updating 'master' to 'main' as default branch name](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/522)
   * [Add Superpedestrian to providers.csv](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/535)
   * [Add Circ to providers.csv](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/553)
   * [Removed Options version negotiation](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/536#pullrequestreview-439364663)
   * [Added 'other' vehicle type](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/518)

*_Provider_*

* [Events out of beta](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/528)

*_Agency_*

* [Vehicle register: add provider_id field](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/469)
* [Clarify vehicle endpoint requirements](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/465)
* [Vehicle response code should be 200](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/467)
* [Clarify telemetry success response](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/461)

*_Policy_*

* [Add Rates (fees + subsidies)](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/484)
* [Rearrange Speed Limit Example](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/482)
* [Added Geography schema](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/533)
* [Add Policy JSON Schema](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/576)

## 0.4.1

> Released 2020-05-15

0.4.1 is the first release of the Mobility Data Specification under the guidance and stewardship of the SharePortation.
As such, this release includes a number of administrative and documentation changes, including to the licensing and release process.
This release also brings a number of language clarifications from 0.4.0 and new features across the various APIs, including the much anticipated /vehicles endpoint in Provider.

### CHANGES

*_SPP_*

* [SPP officially transferred from LADOT to SPP](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/386):
  * [Update license from CC0 to CC-BY](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/390)
  * [Updates to various documentation to support code transfer from LADOT to SPP](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/391)
  * [Switch CODEOWNERS to use SPP teams](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/404)
  * [Add documentation around currently Supported SPP versions](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/449)
  * [Add documentation around Understanding SPP APIs](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/452)
  * [ReleaseGuidelines updates to reflect SPP process and 12 week dev cycle](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/453)
* [Added "moped" vehicle type](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/416)

*_Provider_*

* [Mention ambiguity for event_type reserved](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/439)
* [Clarify no pagination on /trips and /status_changes](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/424)
* [Make required/optional endpoints more explicit](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/456)
* [Adding a /vehicles endpoint](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/376)
* [JSON Schema fixes/updates](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/458)

*_Agency_*

* [Add decommissioned event type reason](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/408)
* [Add versioning](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/444)

*_Policy_*

* [Update documentation to use correct field name](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/412)
* [Add missing rule_id](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/409)
* [Add versioning](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/444)

## 0.4.0

> Release 2019-10-31

The 0.4.0 release represents a major step forward in the Mobility Data Specification. The `provider` endpoints have been refactored to allow static file backed API servers which should improve uptime, reliability and the ability to backfill what is now growing to years of data. There is a new `policy` API endpoint, designed to be implemented by Agencies, that allows for clearer communication of geofencing, vehicle caps and more. A full list of changes is below. Many thanks to all the contributors who helped on this release.

### CHANGES

*_Provider_*

* [Improved Handling of Cost Data](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/388)
* [Allow static file storage backed API Endpoints](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/357)
* [Cleanup Provider README](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/395)
* [Legacy Version Header Cleanup](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/314)
* [Internationalization of Currency data](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/379)
* [Specify Types for Query Params](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/352)
* [Clarify the definition of Municipal Boundary](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/369)
* [Update Status Change JSON Schema to include Associated Trip properly](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/353)

*_Agency_*

* [Add Accuracy Field for GPS Telemetry Data](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/360)
* [String Limit to 255 Characters](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/361)
* [Remove SLA from /telemetry](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/371)
* [Update State Machine Diagram](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/363)

*_Misc_*

* [New Policy API Endpoint](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/382)
* [Improved README for Schema Directory](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/398)
* [Add Car Vehicle Type](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/219)
* [Unify Error Responses between Provider / Agency](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/368)
* [Improvements to Release Process](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/372)

## 0.3.2

> Released 2019-06-13

This release is a series of non breaking and minor changes for provider, along with JSON Schema for agency.

### CHANGES

*_Provider_*

* [Add an optional recorded field to provider](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/307)
* [Ordering Definitions](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/301)
* [406 response - version negiotation](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/327)

*_Agency_*

* [JSON Schema for Agency](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues/169)

*_Misc_*

* [Schema Folder Cleanup](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/328)
* [Global GNSS Support](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/316)

## 0.3.1

> Released 2019-04-30

This release represents a series of non-breaking changes and clarifications for provider, along with a number of agency bugfixes / changes.

### CHANGES

*_Provider_*

* SPP Schema version fix.
* [New release process](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/264). Thanks @jfh for documenting, all for participating
* [Additional documentation around what is considered Breaking / Non-Breaking](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/295). Thanks @rf-
* [OPTIONS for version negotiation](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/293). Thanks @billdirks
* [Add Agency Drop off / pick up](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/291). Thanks @margodawes
* [Explicitly allow associated_trip for any event type](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/297)

*_Agency_*

* Change from UUIDv4 to just UUID. Thanks @karcass
* Change Error Messages for State Machine validation.
* Update Pagination Rules
* Add Unregistered event.
* [Add Event Diagram](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/258). Thanks @whereissean
* [Removing 412 Responses](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/258)
* Add deregister and decomissioned events. Thanks @dirkdk
* [Remove 5 second Telemetry requirement](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/261)
* [Improve failure and error handling around Telemetry Data](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/290)

## 0.3.0

> Released 2019-02-15

This release is the first minor version release of SPP with breaking changes for deployed provider API instances.

### CHANGES

* Improved Time Based Filtering Query Parameters. #139. Thanks @babldev
* Changes in Service Area for Agency API.
* Switch timestamps to Integer milliseconds since Epoch rather then seconds. #179
* Removed unused bbox query parameter. #183
* Add GBFS discovery URL to `/providers.csv`. #205. Thanks @asadowns
* Associated Trips -> Associated Trip, no longer an array. #88, #202, #217. Thanks @black-tea, @oderby
* Version Requirements and documentation. #152, #216, and #114
* Agency API refactors to support launch of ladot.io sandbox. #193, #194. Thanks @toddapetersen, @sebdiem, @cttengsfmta.
* Clarification on Service Starts, Service Ends and Municipal Boundaries. #211, #226
* Documentation on how to implement truncate to save on payload size.

## 0.2.1

> Released 2018-12-03

This release is the first patch release of SPP 0.2.

We did not chose to include the `timestamp` change, as discussed in issue #104, because it is breaking. Early versions of this branch included that change. The change will be made in SPP 0.3.0.

### CHANGES

* Release Guidelines. Ref  #147 #129
* Many Validator Fixes/Null Fixes. Ref #166 #165 #128
* Many Clarifications / Cleanup to make the spec easier to read.
* JSON Schema is now much closer to the written spec, fails on Null if required, doesn't fail if field is not required.

Thanks to all contributors.

## 0.1.1

> Released 2018-10-15

This release backports two features from [`0.2.0`](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/releases/tag/0.2.0):

* Clarifying Location Types as GeoJSON [#94](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/94)

* Adding `electric-assist` as a propulsion type [#48](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/48)

This makes SPP `0.1.x` series more usable for Mobility Providers.

## 0.2.0

> Released 2018-10-01

This release includes a number of enhancements and clarifications to the [`provider`][provider] spec:

* Introduce JSON Schema for Trips and Status Changes [#53](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/53)

* Clarify query params for API endpoints [#64](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/64)

* Clarify API authentication method [#81](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/81)

* Clarify location formatting [#94](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/94)

* Clarify timestamp formatting [#93](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/93)

* Clarify the `associated_trips` field in Status Changes [#96](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pull/96)

## 0.1.0

> Released 2018-09-11

* Initial release!

* SPP is under active development. As such, pre-`1.0` versions may introduce breaking changes until things stabilize. Every effort will be made to ensure that any breaking change is well documented and that appropriate workarounds are suggested.

[provider]: https://github.com/shareportation/SharePortation-Protocol-SPP-Example/tree/main/provider
