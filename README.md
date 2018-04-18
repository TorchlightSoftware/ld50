# LD50

Try it.  It won't kill ya.

## Why should I try it?

You want a backend API.  You want to work as little as possible, and it would be nice if the results were standards compliant.

Or maybe... you are looking into the future of decentralized applications, and you're wondering how we will be storing data in a decentralized way, synchronizing it, and providing access controls and privacy.

## Ok, so what is it?

LD50 is a web-service generator for [JSON-LD](https://json-ld.org/spec/) compliant interfaces.

  * Minimal coding to generate an API - you will mostly supply JSON-LD documents that define the schema, endpoints, policy, and persistence mappings for your data.
  * Define custom services with Javascript.
  * Permissions model based on [LD-OCAP](https://github.com/WebOfTrustInfo/rebooting-the-web-of-trust-fall2017/blob/master/final-documents/lds-ocap.md).
  * OCAP identity verification will rely on an external identity provider (blockchain providers will be primary target, you can mock one out in the meantime)
  * We keep an in-memory representation of a JSON-LD graph, which we serve queries from.
  * We resolve data outside of our local map by retrieving from disk or network.
  * Query language is itself defined in JSON-LD.

![LD50 diagram](docs/LD50.png)
