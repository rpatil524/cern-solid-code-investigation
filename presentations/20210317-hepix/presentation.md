---
type: slide
slideOptions:
  theme: cern
---

HEPiX spring 2021 - CERN-Solid collaboration
===
Maria Dimou (CERN) & Jan Schill (IT University Copenhagen)

Presentation on [March 18th 2021 Storage track](https://indico.cern.ch/event/995485/)

---

## Overview

1. The Solid Ecosystem
  1. Challenges of the Web
  2. What Is Solid?
  3. The Solid Pod
  4. Solid Apps
  5. Solid Implementations
  6. CERN-Solid Code Investigation
2. Demo
  1. Solid Web Server/Pod
  2. Indico Solid Comment Module

---

## Challenges of the Web

*

---

## What Is Solid?

* Sir Tim Berners-Lee (TimBL) announced his Solid project (Social Linked Data) in 2016.
* This Open Source platform aims to re-decentralize the Web and empower users' control over their own data.
* Solid includes standards, missing from the original Web specifications, giving back to the users:
    *  _ownership_ of their _data_, private, shared, and public.
    *  _choice_ on the _storage_ where these data reside and
    *  _control_ over who has _access_ to them.
* TimBL co-founded [inrupt](https://inrupt.com) to implement the Solid standards.

---

## The Solid Pod

* HTTP server
* URI
* Storage
  * RESTful hierarchy
* Linked Data
* Access control
---

### The Solid Pod continued

* A decentralized secure data vault to store **any type of data**.
* Data is store as _Linked Data_, i.e. resource gets its own HTTP URL on the Web
* When data is stored in someone's pod, they control who and what can access it.

(*) Pod: a usually protective container or housing (from the Webster dictionary).

---

## The Solid Servers

1. **Node Solid Server (NSS):** _Open Source_ server by the MIT Solid team since 2016.
2. **Enterprise Solid Server (ESS):** inrupt's commercial _Closed Source_ alternative, based on [Trellis](https://www.trellisldp.org/). Launched in November 2020. [Article](https://sdtimes.com/data/inrupt-launches-enterprise-solid-server-to-restore-trust-in-data/).
3. **Community Solid Server (CSS):** _Open Source_  project by Ghent University, paid for by inrupt, to rewrite NSS from scratch in [TypeScript](https://www.typescriptlang.org/).
5. **php-solid-server (PSS):** _Open Source_, good test results, under dev. The basis for the Nextcloud app that makes Nextcloud compatible with Solid.

---

## Solid servers' interfaces

* All Solid servers have the same common interface, so they don’t need to know anything about what apps are being run on them. See [more here](https://solidproject.org/users/get-a-pod#get-a-pod-from-a-pod-provider)

* Two public demo/test sites for making your own pod. They both run NSS:
    * [inrupt.net](https://inrupt.net/) run by inrupt, hosted at inrupt  premises, USA, data in Amazon Web Services.
    * [solidcommunity.net](https://solidcommunity.net) run by the Solid organisation, hosted in the UK, data in Digital Ocean.
    * a few others people show at the [monthly Solid World Webinar](https://solidproject.org/events).

_Slide with input from TimBL_

---

## Solid implementations

By start-up companies and government agencies. Most engaged countries, so far, are Belgium, the Netherlands, Germany and the UK.
* **Content on the german activities needed here**
* UK NHS (National Health System)
* Flanders' government applications
* Belgian [Digita](https://www.digita.ai/) [inox](https://www.inox.app/) (connects your different pods)
* inrupt developments - [sign-up and play](https://signup.pod.inrupt.com/)

Activities summarised in the [Solid newsletter](https://solidproject.org/newsletter) and reported at the [monthly Solid World Webinar](https://solidproject.org/events).

---

## The CERN-Solid code investigation project

1. **Review Solid specifications**
2. **Evaluate Solid implementations**
3. **Enrich Indico with Solid principles**
4. Recommendations on Solid adoption in CERN applications
5. Document challenges, advantages, gaps
6. Presentation of proceedings

*[Full project description](https://it-student-projects.web.cern.ch/projects/cern-solid-code-investigation)*
*[Very comprehensive report on points 1 & 2 by Jan ](https://indico.cern.ch/event/979244/attachments/2150378/3668572/JanSchill_20201225-Solid-specs-and-implemenations-report.pdf)*
*[GitHub: janschill/cern-solid-code-investigation](https://github.com/janschill/cern-solid-code-investigation)*

---

### Proof of Concept via Indico extensions

![](https://codimd.web.cern.ch/uploads/upload_b81d956728212e88535f5e10e028e371.png)

---

## Conclusion

The success of the [CERN-Solid code investigation project](https://it-student-projects.web.cern.ch/projects/cern-solid-code-investigation) is important:

1. For Jan's MSc thesis at itu.dk to demonstrate that the implementation works.
2. For CERN to be inspired by the PoC and embrace Solid.
    * Solid is there to stay. We should embark now!
4. For Solid to show that its principles can work in an environment of tens of thousands of users.

---

## References Current

* *The Solid project website:* https://solidproject.org
* *Jan's MSc Thesis description:* [https://it-student-projects.web.cern.ch/projects/cern-solid-code-investigation](https://it-student-projects.web.cern.ch/projects/cern-solid-code-investigation)
* *Thesis repo.:* [https://github.com/janschill/uni-research_project](https://github.com/janschill/uni-research_project)
* *CERN-Solid entry point:* [https://indico.cern.ch/category/11962/](https://indico.cern.ch/category/11962/)
* *CERN-Solid chat:* [https://gitter.im/cern-solid/community](https://gitter.im/cern-solid/community)

---

## References Historical

* *The original Web proposal:* https://www.w3.org/History/1989/proposal.html
* *When the CERN Web was Open Source (most data missing today):* https://weboffice.web.cern.ch/WebOffice/
* *Past attempts to involve CERN in W3C work:*
    * *CERN-W3C 2014 proposal:* https://cern.ch/dimou/personal/CERN-W3C_Collaboration.pdf
    * *CERN-W3C 2017 proposal:* https://cern.ch/dimou/personal/CERN-W3C_Collaboration_2017_proposal.pdf