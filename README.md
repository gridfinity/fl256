# fl256

## A high-precision fixed-point numeric representation library for Go

[![License-FL256](https://img.shields.io/badge/Open%20Source%20License-fl256-blue.svg)](https://gitlab.gridfinity.com/jeff/fl256/-/blob/master/LICENSE.256)
[![License-GFODLv1](https://img.shields.io/badge/Proprietary%20License-OX153MkI-red.svg)](https://gitlab.gridfinity.com/jeff/fl256/-/blob/master/LICENSE.153)
[![CodebeatBadge](https://codebeat.co/badges/85330b22-1d38-4937-9fd9-c506098f210e)](https://codebeat.co/projects/github-com-johnsonjh-fl256-master)
[![Maintainability](https://api.codeclimate.com/v1/badges/3c7d3ad4cb992d2cd80d/maintainability)](https://codeclimate.com/github/johnsonjh/fl256/maintainability)

---

### Overview

`fl256` implements a high-precision fixed-point numeric type for Go. It may be
useful in certain domain-specific mathematical contexts.

### Implementation

**NOTE**: This library is built on **big.Float**. As such, it does **not**
implement _end-to-end_ fixed-point calculations, and is **not** using BCD or
other native decimal types. It was originally intended for use in a
crypto-currency ledger system, with specific constraints: a currency with a
maximum supply of 4,398,046,511,103, represented with an unsigned fixed-point
42.214 256-bit interchange format, and is not intended for general purpose
decial calculations or accounting applications.

### Alternatives

Potential users _must_ fully understand the implications and limitations of this
implementation, and evaluate if this system may be appropriate for a particular
application or use case.

There are many mature alternatives that exist for performing financial
calculations using fixed-point operations for general use, such as:

- ["shopspring/decimal"](https://github.com/shopspring/decimal),
- ["cockroachdb/apd"](https://github.com/cockroachdb/apd),
- ["robaho/fixed"](https://github.com/robaho/fixed),
- ["maurodelazeri/go-number"](https://github.com/maurodelazeri/go-number),
- ["lovung/decimal"](https://github.com/lovung/decimal),
- ["ericlagergren/decimal"](https://github.com/ericlagergren/decimal),
- ["umran/money"](https://github.com/umran/money),
- ["db47h/decimal"](https://github.com/db47h/decimal),
- ["wayn3h0/go-decimal"](https://github.com/wayn3h0/go-decimal),
- ["strongo/decimal"](https://github.com/strongo/decimal),
- ["go-info/inf"](https://github.com/go-inf/inf),

Please follow all best practices and industry norms. You must exercise
due diligence when selecting any high precision math library for use.

## Original Author

- [Loki 'l0k18' Verloren](https://github.com/l0k18)
  [\<stalker.loki@protonmail.ch\>](mailto:stalker.loki@protonmail.ch)

  - Loki is the original author of the `float256` library, which `fl256` was
    derived. The source code was released into the public domain, by way of the
    [Unlicense](https://unlicense.org) public domain declaration and dedicaton,
    which [allowed for](https://ar.to/2010/01/dissecting-the-unlicense) the `fl256`
    package to be created, and relicensed, under legally unambigious terms.

## Licensing

`fl256` is distributed as uniquely _multi-licensed software_.

This package is _dual-licensed_, and made available under both a traditional
open-source license, as well as a restricted-use, non-free, proprietary license.

- [***The fl256 License***](https://gitlab.gridfinity.com/jeff/fl256/-/blob/master/LICENSE.256)
  is an Open Source software license. It is _fully compatible_ with
  [***The X.Org Preferred License***](https://gitlab.freedesktop.org/xorg/doc/xorg-docs/-/blob/master/general/License.xml)
  which is a minor variant of [***The MIT License***](https://tldrlegal.com/license/mit-license).
  **The fl256 License** verbiage is identical to that of ***The X.Org Preferred License***,
  differentiated only by changes in punctuation and spacing.

- [***The Oxford 153 Entitlement: Mark I***](https://gitlab.gridfinity.com/jeff/fl256/-/blob/master/LICENSE.153),
  or, informally, "the **OX153MkI**", is a new, unique, non-free, and strongly
  proprietary software license. While the author _strongly_ encourages all eligible
  users to accept the Terms and Conditions of the ***OX153MkI***, it is by no
  means a requirement - anyone who will not (or can not) be bound by the terms
  set forth in the ***OX153MkI*** may fork the repository, and simply remove
  all references to the ***OX153MkI***. In this case, you are bound 
  **ONLY** by the terms of the ***The fl256 License*** open source license. While
  it would be suggested to rename your project to avoid any confusion, there
  is no hard requirement to enforce renaming any derived or forked work.

## Contributing

Anyone who wishes to contribute code (or documentation) to the standard `fl256`
will be required to digitally sign, using either [PGP](https://www.openpgp.org/)
or [opmsg](https://github.com/stealth/opmsg), the "_fl256 CLA/CTA/LO_". This is
a combined Contributor License Agreement, Copyright Transfer Assignment, and Loyalty
Oath. Because of the restrictive Terms and Conditions of **The Oxford 153 Entitlement:
Mark I**, every contributor, no matter how small their contribution, must provide the
*fl256 authors* a digitally signed copy of the "_fl256 CLA/CTA/LO_" document without
exception.

The Contributor License Agreement, Copyright Transfer Assignment, and Loyalty Oath
is intended to ensure, in perpetuity, the absolute integrity of any and all tools
distributed under the **OX153MkI**. As such, this is a non-negotiable, eternally
binding legal instrument, by which the contributor grants the *the fl256 authors"
a perpetual, world- and universe-wide, non-exclusive, free-of-charge, zero-royalty,
forever irrevocable, persistent, immutable, absolute, unalterable, and completely
unlimited-in-scope license to the contribution, as well as a complete and total
assignment of copyright and ownership, which allows *the fl256 authors* to reproduce,
redistribute, sub-license, re-license, or otherwise fully control the contribution,
in it's entirety, including any works which may be later derived from the
contribution. The document also includes a specific Loyalty Oath, intended to formally
and authoritatively finalize total acceptance of, and assure eternal adherence to, the
principles and values embodied by the **The Oxford 153 Entitlement: Mark I**.

A complete copy of "_fl256 CLA/CTA/LO_" will be furnished upon request to any potential
contributors. We encourage all potential contributors read and completely understand the
the "_fl256 CLA/CTA/LO_". It this recommended that would-be contributors seek the guidance
from licensed and qualified legal council, well-versed in such matters, as they  would be
best qualified to offer any necessary assistance or clarity if any questions should arise
during your review of the "_fl256 CLA/CTA/LO_" documents. Unfortunately, we can not, and
will not, answer any inquiry regarding the content of the "_fl256 CLA/CTA/LO_" document.
