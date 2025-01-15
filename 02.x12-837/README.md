```
camel run --dep=org.smooks.cartridges:smooks-dfdl-cartridge:1.0.1 X12-837P* 837-to-xml*
```

or

```
camel run --dep=org.smooks.cartridges:smooks-dfdl-cartridge:1.0.1 X12-837P* xml-to-837*
```


Also possible to raise log level and/or enable JVM debugger for debugging purpose, for example
```
camel run --dep=org.smooks.cartridges:smooks-dfdl-cartridge:1.0.1 X12-837P* 837-to-xml* --logging-category=org.apache.daffodil=DEBUG --jvm-debug
```
