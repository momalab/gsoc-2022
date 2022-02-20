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
- [Standardization of the E3 framework core and settings](#standardization-of-the-e3-framework-core-and-settings)
- [Design a test suite for the E3 framework](#design-a-test-suite-for-the-e3-framework)


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

### Standardization of the E3 framework core and settings

Fully Homomorphic Encryption (FHE) enables computation to be performed directly on encrypted data. Several FHE encryption schemes and supporting libraries have been proposed in recent years, each one with its own API and encryption parameters. Aiming at facilitating access to encrypted computation to non-crypto programmers and increasing the portability of FHE applications, MoMA Lab has developed the E3 framework.
The E3 framework works at a higher level of abstraction than FHE libraries. It decouples the cryptography parameters from the programming part and enables the same code to be used across different FHE libraries.
Furthermore, E3 offers secure data types to be used in a C++ program similarly to how a programmer uses integers or an array of integers in SIMD programming.
Each library underneath E3 has its own naming convention for encryption parameters, which at the moment is passed to the crypto expert for setting up E3. One goal of this project is to standardize these parameters to be the same across different libraries and, if possible, across different encryption schemes.
In addition, we would like to improve the internals of the CGT tool, a tool part of E3 that generates the secure data types to natively support encoded arrays of plaintexts as polynomials, which we believe may increase performance for some FHE applications.

#### Expected Outcome
- Configuration of cryptographic parameters will be standard for all underneath libraries and encryption schemes
- New data types for better programming and improved performance will be available
- Internals of E3 will be standardized


#### Required Skills
Experience with C++

#### Preferred Skills
Understanding of data-oblivious programming

#### Possible Mentors
Eduardo Chielle, Oleg Mazonka

#### Repository
[github.com/momalab/e3](github.com/momalab/e3)

#### Project Size
Large Project (~350 hours of work)

#### Difficulty Rating
Hard

---

### Design a test suite for the E3 framework

Fully Homomorphic Encryption (FHE) enables computation to be performed directly on encrypted data. Several FHE encryption schemes and supporting libraries have been proposed in recent years, each one with its own API and encryption parameters. Aiming at facilitating access to encrypted computation to non-crypto programmers and increasing the portability of FHE applications, MoMA Lab developed the E3 framework.
The E3 framework works at a higher level of abstraction than FHE libraries. It decouples the cryptography parameters from the programming part and enables the same code to be used across different FHE libraries.
Our framework is in constant development, with new encryption libraries and schemes being added, inclusion of new features and tools, and improvements to internals.
Every modification to E3 requires testing to guarantee that all features are working properly. With this object, we would like this project to develop a comprehensive testing suite for the E3 covering all operations available to the user.

#### Expected Outcome
A test suite will be designed for the E3 framework that will cover all user available operations and ensure their proper functioning.

#### Required Skills
Experience with C++

#### Preferred Skills
Understanding of data-oblivious programming

#### Possible Mentors
Eduardo Chielle, Oleg Mazonka

#### Repository
[github.com/momalab/e3](github.com/momalab/e3)

#### Project Size
Large Project (~350 hours of work)

#### Difficulty Rating
Medium

---