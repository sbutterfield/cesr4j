# CESR JavaEE low-level library

**Project Name:** cesr4j
This is the home of a Java native implementation of the CESR encoding format.

## What is CESR?
The Composable Event Streaming Representation (CESR) is dual text- binary encoding format that has the unique property of text-binary concatenation composability. This composability property enables the round trip conversion en-masse of concatenated primitives between the text domain and binary domain while maintaining separability of individual primtives. This enables convenient usability in the text domain and compact transmission in the binary domain. CESR primitives are self-framing. CESR supports self-framing group codes that enable stream processing and pipelining in both the text and binary domains. CESR supports composable text-binary encodings for general data types as well as suites of cryptographic material. Popular cryptographic material suites have compact encodings for efficiency while less compact encodings provide sufficient extensibility to support all foreseeable types. CESR is a universal encoding that uniquely provides dual text and binary domain representations via composable conversion.

## What does this library do?
With a few transitive dependencies as possible, this library aims to provide a narrow implementation surface with deep functions to support interleaved, multi-domain encoding support for JSON and CBOR serializations into and out of CESR encoding.

Because CESR is a new composable encoding specification that works across text and binary domains, it's uniquely suited to deal with transmission compatibility for cryptographic material - like Authentic Chained Data Containers, or Key Events in KERI. The possible uses for CESR are very broad, so this library is super unopinionated about how you choose to implement it.

## Build
This project is built with Bazel. You can read more about that here: https://bazel.build/