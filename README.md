# SharePortation

## Table of Contents

- [About](#about)
- [Endpoints](#endpoints)
  - [Modularity](#modularity)
  - [GBFS Requirement](#gbfs-requirement)
- [Get Involved](#get-involved)
  - [Membership](#membership)  
- [Versions](#versions)
  - [Technical Information](#technical-information)
- [Cities Using SPP](#cities-using-SPP)
- [Providers Using SPP](#providers-using-SPP)
- [Software Companies Using SPP](#software-companies-using-SPP)
- [Data Privacy](#data-privacy)
- [Use Cases](#use-cases)
- [Related Projects](#related-projects)

# About

The SharePortation (**SPP**), a project of the [SharePortation](http://www.shareportation.org) (**SPP**), is a set of Application Programming Interfaces (APIs) focused on shared mobility services such as dockless scooters, bicycles, mopeds, and carshare, and inspired by projects like [GTFS](https://developers.google.com/transit/gtfs/reference/) and [GBFS](https://github.com/NABSA/gbfs). SPP is a digital tool that helps cities better manage transportation in the public right of way, standardizing communication and data-sharing between cities and private mobility providers, allowing cities to share and validate policy digitally, and enabling vehicle management and better outcomes for residents. 

**SPP** is a key piece of digital infrastructure that supports the effective implementation of mobility policies in cities around the world. For a high level overview and visuals, see the [About SPP](https://www.shareportation.org/about-SPP/) page on the SPP website.

![SPP master Logo](https://i.imgur.com/zFvzQn1.png)

**SPP** is an open-source project originally created by the [Los Angeles Department of Transportation](http://ladot.io) (LADOT). In November 2019, stewardship of SPP and the ownership of this repository were transferred to the [SharePortation](http://www.shareportation.org). GitHub automatically redirects any links to this repository from the `CityOfLosAngeles` organization to the `shareportation` instead. SPP continues to be used by LADOT and [many other municipalities](#cities-using-SPP) and companies.

[Top][toc]

# Endpoints

**SPP** is comprised of six distinct APIs, with multiple endpoints under each API:

<a href="/provider/"><img src="https://i.imgur.com/zFvzQn1.png" width="80" align="left" alt="SPP Provider Icon" border="0"></a>

The [`provider`][provider] API endpoints are intended to be implemented by mobility providers and consumed by regulatory agencies. When a municipality queries information from a mobility provider, the Provider API has a historical view of operations in a standard format. It was first released in June 2018. 

---

<a href="/agency/"><img src="https://i.imgur.com/zFvzQn1.png" width="80" align="left" alt="SPP Agency Icon" border="0"></a>

The [`agency`][agency] API endpoints are intended to be implemented by regulatory agencies and consumed by mobility providers. Providers query the Agency API when events (such as a trip start or vehicle status change) occur in their systems. It was first released in April 2019. 

---

<a href="/policy/"><img src="https://i.imgur.com/zFvzQn1.png" width="80" align="left" alt="SPP Policy Icon" border="0"></a>

The [`policy`][policy] API endpoints are intended to be implemented by regulatory agencies and consumed by mobility providers. Providers query the Policy API to get information about local rules that may affect the operation of their mobility service or which may be used to determine compliance. It was first released in October 2019.

---

<a href="/geography/"><img src="https://i.imgur.com/zFvzQn1.png" width="80" align="left" alt="SPP Geography Icon" border="0"></a>

The [`geography`][geography] API endpoints are intended to be implemented by regulatory agencies and consumed by mobility providers. Providers query the Policy API to get information about geographical regions for regulatory and other purposes. It was first released in October 2019, originally included as part of the Policy specification. 

---

<a href="/jurisdiction/"><img src="https://i.imgur.com/zFvzQn1.png" width="80" align="left" alt="SPP Jurisdiction Icon" border="0"></a>

The [`jurisdiction`][jurisdiction] API endpoints are intended to be implemented by regulatory agencies that have a need to coordinate with each other. The jurisdiction endpoints allow cities to communicate boundaries between one another and to mobility providers. It was first released in March 2021. 

---

<a href="/metrics/"><img src="https://i.imgur.com/zFvzQn1.png" width="80" align="left" alt="SPP Metrics Icon" border="0"></a>

The [`metrics`](/metrics) API endpoints are intended to be implemented by regulatory agencies or their appointed third-party representatives to have a standard way to consistently describe available metrics, and create an extensible interface for querying SPP metrics. It was first released in March 2021. 

---

## Modularity

SPP is designed to be a modular kit-of-parts. Regulatory agencies can use the components of the API that are appropriate for their needs. An agency may choose to use only `agency`, `provider`, or `policy`. Other APIs like `geography`, `jurisdiction`, and `metrics` can be used in coordination as described with these APIs or sometimes on their own. Or agencies may select specific elements (endpoints) from each API to help them implement their goals. Development of the APIs takes place under the guidance of the SPP's [SPP Working Group](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki/SPP-Working-Group).

Many parts of the SPP definitions and APIs align across each other. In these cases, consolidated information can be found on the [General Information](/general-information.md) page.

You can read more in our **[Understanding the different SPP APIs](https://github.com/shareportation/governance/blob/master/technical/Understanding-SPP-APIs.md)** guide. 

![SPP APIs and Endpoints](https://i.imgur.com/zFvzQn1.png)

## GBFS Requirement

All SPP compatible Provider feeds [must also expose](/provider/README.md#gbfs) a public [GBFS](https://github.com/NABSA/gbfs) feed. Compatibility with [GBFS 2.0](https://github.com/NABSA/gbfs/blob/v2.0/gbfs.md) or greater is advised due to privacy concerns and support for micromobility. See our [SPP Vehicles Guide](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki/SPP-Vehicles) for how SPP Provider `/vehicles` can be used by regulators instead of the public GBFS `/free_bike_status`. Additional information on SPP and GBFS can be found in this [guidance document](https://github.com/shareportation/governance/blob/master/technical/GBFS_and_SPP.md).

[Top][toc]

# Get Involved

To stay up to date on SPP, please **subscribe to the [SPP-announce](https://groups.google.com/a/groups.shareportation.org/g/SPP-announce) mailing list** for general updates, the **[wg-SPP](https://groups.google.com/a/groups.shareportation.org/g/wg-SPP) mailing list** for Working Group details and meetings, and read our **[Community Wiki](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki)**.

The SharePortation is an open source project with all development taking place on GitHub and public meetings through our [SPP Working Group](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki/SPP-Working-Group). Comments and ideas can be shared by [starting a discussion](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/discussions), [creating an issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues), suggesting changes with [a pull request](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pulls), and attending meetings. Before contributing, please review our SPP [CONTRIBUTING](https://github.com/shareportation/governance/blob/master/CONTRIBUTING.md) and [CODE OF CONDUCT](https://github.com/shareportation/governance/blob/master/CODE_OF_CONDUCT.md) pages to understand guidelines and policies for participation.

**Read our [How to Get Involved in the SharePortation](https://www.shareportation.org/how-to-get-involved-in-the-open-mobility-foundation/) blog post for more detail and an overview of how the SPP is organized.**

For other questions about SPP or media inquiries please contact the SPP directly [on our website](https://www.shareportation.org/get-in-touch/). 

## Membership

SPP Members (public agencies and commercial companies) have additional participation opportunities with leadership roles within our SPP [governance](https://github.com/shareportation/governance#SPP-scope-of-work):

- [Board of Directors](https://www.shareportation.org/about/)
- [Privacy, Security, and Transparency Committee](https://github.com/shareportation/privacy-committee)
- [Technology Council](https://github.com/shareportation/governance/wiki/Technology-Council)
- [Strategy Committee](https://github.com/shareportation/governance/wiki/Strategy-Committee)
- [Advisory Committee](https://github.com/shareportation/governance/wiki/Advisory-Committee)
- Steering committees of all [Working Groups](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki#SPP-meetings), currently:
  - [SPP Working Group](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki/SPP-Working-Group)
  - [Curb Working Group](https://github.com/shareportation/curb-data-specification/wiki)

Read about [how to become an SPP member](https://www.shareportation.org/how-to-become-a-member/), [how to get involved and our governance model](https://www.shareportation.org/how-to-get-involved-in-the-open-mobility-foundation/), and [contact us](https://mailchi.mp/shareportation/membership) for more details. 

[Top][toc]

# Versions

SPP has a **current release** (version 1.2.0), **previous releases** (both recommended and longer recommended for use), and **upcoming releases** in development. For a full list of releases, their status, recommended versions, and timelines, see the [Official SPP Releases](https://github.com/shareportation/governance/wiki/Releases) page.

The SPP provides guidance on upgrading for cities, providers, and software companies, and sample permit language for cities. See our [SPP Version Guidance](https://github.com/shareportation/governance/blob/master/technical/SPP-SPP-Version-Guidance.md) for best practices on how and when to upgrade SPP as new versions become available. Our complimentary [SPP Policy Language Guidance](https://github.com/shareportation/governance/blob/master/technical/SPP-SPP-Policy-Language-Guidance.md) document is for cities writing SPP into their operating policy and includes sample policy language.

## Technical Information

The latest SPP release is in the [`master`](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/tree/master) branch, and development for the next release occurs in the [`dev`](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/tree/dev) branch.

The SPP specification is versioned using Git tags and [semantic versioning](https://semver.org/). See prior [releases](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/releases) and the [Release Guidelines](https://github.com/shareportation/governance/blob/master/technical/ReleaseGuidelines.md) for more information and [version support](https://github.com/shareportation/governance/blob/master/technical/ReleaseGuidelines.md#ongoing-version-support).

* [Latest Release Branch](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/tree/master) (master)
* [Development Branch](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/tree/dev) (dev)
* [All GitHub Releases](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/releases)
* [SPP Releases](https://github.com/shareportation/governance/wiki/Releases) - current/recommended versions, timeline
* [Release Guidelines](https://github.com/shareportation/governance/blob/master/technical/ReleaseGuidelines.md)

[Top][toc]

# Cities Using SPP

More than 150 cities and public agencies across 6 continents around the world use SPP, and it has been implemented by most major [mobility service providers](#providers-using-SPP).  
- See our **[list of cities using SPP](https://www.shareportation.org/SPP-users/#cities-using-SPP)** with links to public mobility websites and policy/permit documents.

Please let us know [via our website](https://www.shareportation.org/get-in-touch/) or in the [public discussion area](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/discussions) if you are an agency using SPP so we can add you to the city resource list, especially if you have published your policies or documents publicly.

To add yourself to the [agency list](/agencies.csv) and add your [Policy Requirement link](/provider.md#requirements), please let us know [via our website](https://www.shareportation.org/get-in-touch/) or open an [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues) or [Pull Request](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pulls). Find out how in our [Adding an Agency ID](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki/Adding-an-SPP-Agency-ID) help document.

[Top][toc]

# Providers Using SPP

Over two dozen mobility service providers (MSPs) around the world use SPP, allowing them to create tools around a single data standard for multiple cities. 

- See our **[list of providers using SPP](https://www.shareportation.org/SPP-users/#mobility-providers-using-SPP)**. For a table list with unique IDs, see the SPP [provider list](/providers.csv).

To add yourself to the provider list, please let us know [via our website](https://www.shareportation.org/get-in-touch/) or open an [Issue](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/issues) or [Pull Request](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/pulls). Find out how in our [Adding an Provider ID](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki/Adding-an-SPP-Provider-ID) help document.

[Top][toc]

# Software Companies Using SPP

An open source approach to data specifications benefits cities and companies by creating a space for collaborative development, reducing costs, and nurturing a healthy, competitive ecosystem for mobility services and software tools. The open model promotes a competitive ecosystem for software tools built by dozens of software companies providing their services to cities, agencies, and providers.

- See our **[list of third party software companies using SPP](https://www.shareportation.org/SPP-users/#software-companies-using-SPP)** and an article about the [benefits of an open approach](https://www.shareportation.org/why-open-behind-SPPs-unique-open-source-model/). 

Please [let us know](https://www.shareportation.org/get-in-touch/) if you are using SPP in your company so we can add you to the list.

[Top][toc]

# Data Privacy

SPP includes information about vehicles, their location, and trips taken on those vehicles to allow agencies to regulate their use in the public right of way and to conduct transportation planning and analysis. While SPP is not designed to convey personal information about the users of shared mobility services, data collected about mobility can be sensitive. The SPP and SPP community have created a number of resources to help cities, mobility providers, and software companies handle vehicle data safely:

* [SPP Privacy Guide for Cities](https://github.com/shareportation/governance/raw/master/documents/SPP-SPP-Privacy-Guide-for-Cities.pdf) - guide that covers essential privacy topics and best practices
* [The Privacy Principles for Mobility Data](https://www.mobilitydataprivacyprinciples.org/) - principles endorsed by the SPP and other mobility organizations to guide the mobility ecosystem in the responsible use of data and the protection of individual privacy
* [Mobility Data State of Practice](https://github.com/shareportation/privacy-committee/blob/master/products/state-of-the-practice.md) -  real-world examples related to the handling and protection of SPP and other types of mobility data
* [Understanding the Data in SPP](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/wiki/Understanding-the-Data-in-SPP) - technical document outlining what data is (and is not) in SPP
* [Use Case Database](https://www.shareportation.org/whats-possible-with-SPP/) - a starting point for understanding how SPP can be used, and what parts of SPP is required to meet those use cases
* [Policy Requirements](https://github.com/shareportation/SharePortation-Protocol-SPP-Example/tree/master/policy#requirement) - built into SPP, allowing agencies to specify only the endpoints and fields needed for program regulation
* Using SPP Under GDPR (link coming soon) - how to use SPP in the context of GDPR in Europe

The SPP’s [Privacy, Security, and Transparency Committee](https://github.com/shareportation/privacy-committee#welcome-to-the-privacy-security-and-transparency-committee) creates many of these resources, and advises the SPP on principles and practices that ensure the secure handling of mobility data. The committee – which is composed of both private and public sector SPP members – also holds regular public meetings, which provide additional resources and an opportunity to discuss issues related to privacy and mobility data. Learn more [here](https://github.com/shareportation/privacy-committee#welcome-to-the-privacy-security-and-transparency-committee).

[Top][toc]

# Use Cases

How cities use SPP depends on a variety of factors: their transportation goals, existing services and infrastructure, and the unique needs of their communities. Cities are using SPP to create policy, enforce rules, manage hundreds of devices, and ensure the safe operation of vehicles in the public right of way. Some examples of how cities are using SPP in practice are:

- **Vehicle Caps:** Determine total number of vehicles per operator in the right of way
- **Distribution Requirements:** Ensure vehicles are distributed according to equity requirements
- **Injury Investigation:** Investigate injuries and collisions with other objects and cars to determine roadway accident causes
- **Restricted Area Rides:** Find locations where vehicles are operating or passing through restricted areas
- **Resident Complaints:** Investigate and validate complaints from residents about operations, parking, riding, speed, etc, usually reported through 311
- **Infrastructure Planning:** Determine where to place new bike/scooter lanes and drop zones based on usage and demand, start and end points, and trips taken

A list of use cases is useful to show what's possible with SPP, to list what other cities are accomplishing with the data, to see many use cases up front for privacy considerations, and to use for policy discussions and policy language. More details and examples can be seen on the [SPP website](https://www.shareportation.org/whats-possible-with-SPP/) and our [Wiki Database](https://github.com/shareportation/governance/wiki/SPP-Use-Cases).

Please [let us know](https://docs.google.com/forms/d/e/1FAIpQLScrMPgeb1TKMYCjjKsJh3y1TPTJO8HR_y1NByrf1rDmTEJS7Q/viewform) if you have recommended updates or use cases to add.

[Top][toc]

# Related Projects

Community projects are those efforts by individual contributors or informal groups that take place outside SharePortation’s formalized process, complementing SPP. These related projects often push new ideas forward through experimental or locally-focused development, and are an important part of a thriving open source community. Some of these projects may eventually be contributed to and managed by the SharePortation.

The SPP's [Communitiy Projects](https://www.shareportation.org/community-projects/) page has an every growing list of projects related to SPP, and see our [Privacy Committee's State of Practice](https://github.com/shareportation/privacy-committee/blob/master/products/state-of-the-practice.md) for more examples.

Please [let us know](https://www.shareportation.org/get-in-touch/) if you create open source or private tools for implementing or working with SPP data.

[Top][toc]

[agency]: /agency/README.md
[provider]: /provider/README.md
[policy]: /policy/README.md
[geography]: /geography/README.md
[jurisdiction]: /jurisdiction/README.md
[metrics]: /metrics/README.md
[toc]: #table-of-contents
