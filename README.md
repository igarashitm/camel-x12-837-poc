# X12 837 message handling with Camel PoC

The purpose of this PoC is to demonstrate reading and writing X12 837 EDI message in Camel Route with using Smooks DFDL support, as well as letting Kaoto DataMapper participate in.

## TODO

- [x] Take Smooks edi-to-xml and xml-to-edi examples in to [](01.camel-smooks-edi-xml-example) and wrap into camel routes
- [x] Verify both edi-to-xml and xml-to-edi works
- [x] Copy [Smooks example files](01.camel-smooks-edi-xml-example) into [working dir](02.x12-837) and rename them to represent X12 837 usecase
- [x] Start making hands dirty - replace the example input payloads with X12 837 (input for 837-to-xml, output for xml-to-837)
- [ ] Create the example XML (output for 837-to-xml, input for xml-to-837) which represents the example X12 837 above
- [ ] Update DFDL schema files to reflect those 837 and XML formats
- [ ] Make sure it runs and prints the log as expected
- [ ] Add DataMapper, so not only just convert between X12 837 and XML, but also demonstrate to read/write from/to a different data shape
- [ ] Verify it runs and prints the log as expected

## Contents
1. [01.camel-smooks-edi-xml-example](01.camel-smooks-edi-xml-example)
Just a reference, copied the Smooks example in and wrapped into camel route. It is using EDIFACT common object. A starting point.
2. [02.x12-837](02.x12-837)
A working directory. Using [above](01.camel-smooks-edi-xml-example) as a template, create 2 camel routes to demonstrate to read/write X12 837 message, as well as performing data mapping on it.
