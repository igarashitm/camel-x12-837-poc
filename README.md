# X12 837 message handling with Camel PoC

The purpose of this PoC is to demonstrate reading and writing X12 837 EDI message in Camel Route with using Smooks DFDL support, as well as letting Kaoto DataMapper participate in.

## TODO

- [x] Take Smooks edi-to-xml and xml-to-edi examples in to [](01.camel-smooks-edi-xml-example) and wrap into camel routes
- [x] Verify both edi-to-xml and xml-to-edi works
- [ ] Copy [Smooks example files](01.camel-smooks-edi-xml-example) into [working dir](02.x12-837) and rename them to represent X12 837 usecase
- [ ] Start making hands dirty - replace the example input payloads with X12 837
- [ ] And update DFDL schema files to handle X12 837 format
- [ ] Make sure it runs and prints the log as expected
- [ ] Add DataMapper, so not only just convert between X12 837 and XML, but also demonstrate to read/write from/to a different data shape
- [ ] Verify it runs and prints the log as expected

## Contents
1. [01.camel-smooks-edi-xml-example](01.camel-smooks-edi-xml-example)
Just a reference, copied the Smooks example in and wrapped into camel route. It is using EDIFACT common object. A starting point.
2. [02.x12-837](02.x12-837)
A working directory. Using [above](01.camel-smooks-edi-xml-example) as a template, create 2 camel routes to demonstrate to read/write X12 837 message, as well as performing data mapping on it.
