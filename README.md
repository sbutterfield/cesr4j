# CESR JavaEE low-level library

**Project Name:** cesr4j
This is the home of a Java native implementation of the CESR encoding format.

## What is CESR?
The Composable Event Streaming Representation (CESR) is dual text- binary encoding format that has the unique property of text-binary concatenation composability. This composability property enables the round trip conversion en-masse of concatenated primitives between the text domain and binary domain while maintaining separability of individual primtives. This enables convenient usability in the text domain and compact transmission in the binary domain. CESR primitives are self-framing. CESR supports self-framing group codes that enable stream processing and pipelining in both the text and binary domains. CESR supports composable text-binary encodings for general data types as well as suites of cryptographic material. Popular cryptographic material suites have compact encodings for efficiency while less compact encodings provide sufficient extensibility to support all foreseeable types. CESR streams also support interleaved JSON, CBOR, and MGPK serializations. CESR is a universal encoding that uniquely provides dual text and binary domain representations via composable conversion.