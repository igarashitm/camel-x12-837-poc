```
camel run --dep=org.smooks.cartridges:smooks-dfdl-cartridge:1.0.1 837-to-xml*
```

or

```
camel run --dep=org.smooks.cartridges:smooks-dfdl-cartridge:1.0.1 xml-to-837*
```


Also possible to raise log level and/or enable JVM debugger for debugging purpose, for example
```
camel run --dep=org.smooks.cartridges:smooks-dfdl-cartridge:1.0.1 837-to-xml* --logging-category=org.apache.daffodil=DEBUG --jvm-debug
```