#### EDI to XML
```
camel run X12-837P* 837-to-xml*
```

or

#### XML to EDI
```
camel run X12-837P* xml-to-837*
```

or

#### EDI to XML + Kaoto DataMapper
```
camel run X12-837P.dfdl.xsd x12-837-datamapper.camel.yaml kaoto-datamapper-2df1aa0e.xsl 837-to-xml-input-message.edi
```

#### misc   

Also possible to raise log level and/or enable JVM debugger for debugging purpose, for example
```
camel run X12-837P* 837-to-xml* --logging-category=org.apache.daffodil=DEBUG --jvm-debug
```
