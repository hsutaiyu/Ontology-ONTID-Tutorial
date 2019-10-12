---
description: A brief description of the ONT ID framework and what it can be used to achieve
---

# Introduction

The ONT ID framework aims at providing:

1. A **self-sovereign** identity for web applications, turning the end user\(s\) into a stakeholder\(s\)
2. A platform to match the target users for web apps via a collection of **third party claims**, thereby creating a **trust mechanism** of Ontology.

## Self sovereign identity

To make the context clear when talking about entities in terms of Ontology's ONT ID framework, let us lay out the various kinds of entities that the ONT ID framework can work with:

* Individuals
* Legal Entities - Organizations, enterprises, institutions, etc.
* Objects - Mobile phones, automobiles, IoT devices, etc.
* Content - Creative content that can be copyrighted or patented

{% hint style="warning" %}
Within the scope of ONT ID's system, the term **identity** refers to a given entity's identity withing the trust network.
{% endhint %}

1. **ONT ID** serves as the identifier in the ONT ID identification framework. All entities in Ontology system will have a unique `ONT ID`. Ontology uses this identifier to associate and manage the entities' identities. On the Ontology blockchain one entity can correspond to multiple individual identities, and there is no relation between such identities.
2. **ONT Auth** is the mechanism implemented as an application that is used to enable the self sovereign identification process for the `ONT ID` services deployed on the Ontology `mainnet`.
3. **Signing server** is a server side back end service used to bridge the `ONT ID` from the user to the account system inside a web app.

### Workaround for centralized businesses

In order to satisfy the users acquainted with using traditional web apps, some web apps may start with a centralized ID business logic. **ONT ID** framework provides a solution to the above problem so as to allow web apps to meet any necessary requirements.

The centralized identifiers can be handed back to the **ONT ID** owners by altering the `owner` of `ONT ID`  in the **DID Descriptor Object** \(DDO\) from web app to the end user.

{% hint style="warning" %}
For more details on the **W3C** standard for **Decentralized Identifiers** \(DID\) protocol please follow [this](https://w3c-ccg.github.io/did-spec/) link.
{% endhint %}

## Ontology trust mechanism

Entities issue claims and "sell" them to their customers, who then utilize them under various verification scenarios. The closed loop of issuing requests, creation and consumption of claims sets up Ontology's **trust mechanism**.

Ontology employs the **credible declaration** technology to realize and implement the trust mechanism.

The components that serve as the framework to implement the mechanism are described below:

1. **Trust Anchor -** Refers to the entity that provides authentication services on the Ontology ecosystem. Institutions such as, but not limited to - government agencies, universities, banks, third party authentication service agencies \(such as CA\) or biometric technology companies.
2. **Claim store -** An entity that provides an online "claim management" service and performs functions such as notifying the claim `owner` when there is an interested claim `consumer` for certain credentials. A claim store is generally an entity that adheres to a non-disclosure agreement \(NDA\) so as to ensure data privacy.
3. **ONT Auth -** A mobile application designed with the specific goal of personal claim management.



