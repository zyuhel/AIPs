---
aip: <to be assigned>
title: URI Format for ADAMANT Contact Links
author: Dmitriy Soloduhin (@zyuhel) and Pavel Anokhov (@RealBonus)
discussions-to: <to be added>
status: Draft
type: Standards
category: ARC
created: 2018-06-23
requires: 2
---

<!--You can leave these HTML comments in your merged AIP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new AIPs. Note that an AIP number will be assigned by an editor. When opening a pull request to submit your AIP, please use an abbreviated title in the filename, `aip-draft_title_abbrev.md`. The title should be 44 characters or less.-->

## Simple Summary
Argument and parameters list for ADM URI regarding contact data. 

## Abstract
<!--A short (~200 word) description of the technical issue being addressed.-->
This AIP extends [AIP-2](https://aips.adamant.im/AIPS/aip-2) and defines parameters for ADAMANT Contact URIs.

## Motivation
<!--The motivation is critical for AIPs that want to change the protocol. It should clearly explain why the existing protocol specification is inadequate to address the problem that the AIP solves. AIP submissions without sufficient motivation may be rejected outright.-->
Help integrating ADAMANT into world. Standartise URIs between different ADAMANT Messenger realization. 

## Specification
<!--The technical specification should describe the syntax and semantics of any new feature. The specification should be detailed enough to allow competing, interoperable implementations for different platforms.-->
### Syntax
Possible parameters
```
label                   = uri encoded string
message                 = uri encoded string

```

### Semantics
`label` is recommended optional parameter, it is shown how address former wants to be listed in Address Book of users clicking on the link. Obeying this parameter is on conscience of ADAMANT Messenger realization, because this field could possibly be used for phishing.
Also label value MUST NEVER be same as ADAMANT address format. 
`message` is optional parameter, it's behaviour is same as `body` argument of mailto: protocol. 



## Rationale
<!--The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.-->
This ARC is needed to ensure that all ADAMANT Messengers realizations support same URI format.


## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
