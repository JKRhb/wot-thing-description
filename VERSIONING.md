# Versioning of TD Specification Resources

In addition to the specifications, there are other resources that are managed in this repository.
This file documents the discussion on how the versioning should be.
Once there is an agreement, the rules will be moved to [wot-resources](https://github.com/w3c/wot-resources) repository.
The points below present a summary, but you can scroll to the bottom of the page to find the original input from the meetings.

- With each REC, we publish the following files:
  -  Ontology files in form of TTL and HTML. These are TD, Security, hypermedia controls, JSON Schema, and soon the TM
  -  JSON-LD Context file
  -  JSON Schemas for TD and TM
-  We do not publish different versions of these files until we see the need (e.g. a bug that also has breaking changes to current implementations).
-  

## Original Input

Text copied from <https://www.w3.org/WoT/IG/wiki/WG_WoT_Thing_Description_WebConf>

- What do we mean by versioning?
  - Pointing to the most recent version but also older versions should be available
  - Semver with Major, Minor, Patch at semver.org
  - For TD.next, do we want to publish resources with each publication (WD, CR, PR etc) or not?
- Which changes are bugfixes, new features (TD 2.0 keywords)
  - JSON Schemas
    - Patch: English typos etc. Minor: Relaxing a constraint (longer strings, more oneof) so that more TDs can pass the schema. Major: Adding or restricting constraints
  - JSON-LD Context
  - Ontology files
    - TTL
    - HTML
- How much time to invest in maintaining 1.1 resources?
– Maintaining multiple files or not: xxx.v1.1.0.ttl xxx.v1.1.1.ttl
- Decision so far: Do not dig into 1.1 versioning until we have the need.
- TM resources (tm.ttl and tm.html) will not be versioned for the first changes since HTML doesn't exist and TTL is not usable.
