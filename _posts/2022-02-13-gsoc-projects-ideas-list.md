---
layout: post
title: "GSoC 2022 Project Ideas List"
description: "Ideas for Google Summer of Code 2022 Proposals."
thumb_image: "documentation/sample-image.jpg"
tags: [ideas]
---

The ideas on the list presented in this page pertain to Open Source projects actively maintained by MoMA. While this list is meant to inspire Contributors to submit their proposals, it is by no means exhaustive and MoMA welcomes proposals for ideas beyond it.

## Index
- [Extending ICSREF to support Codesys V3 binaries](#extending-icsref-to-support-codesys-v3-binaries)



---

### Extending ICSREF to support Codesys V3 binaries

Industrial Control Systems (ICS) play an important role in monitoring, automating and controlling manufacturing, energy and critical infrastructure processes (e.g: water desalination, smart energy grids, assembly lines etc.).
Devices found in ICS like Programmable Logic Controllers (PLCs) are programmed using domain specific programming languages, such as Structured Text,  that are compiled to specialty vendor binaries.
ICSREF is a Reverse Engineering framework for ICS binaries that is used extensively by the ICS security research community.
The framework initially enabled reverse engineering Codesys V2 binaries, but has the ability to be extended to support binaries of the newer Codesys V3 runtime.

#### Expected Outcome
ICSREF will be extended to support reverse engineering Codesys V3 ICS binaries.

#### Required Skills
Python

#### Preferred Skills
Experience with radare2 and Angr

#### Possible Mentors
Michail Maniatakos, Constantine Doumanidis, Prashant Rajput

#### Repository
[https://github.com/momalab/ICSREF](https://github.com/momalab/ICSREF)

#### Project Size
Large Project (~350 hours of work)

#### Difficulty Rating
Hard

---