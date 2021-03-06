# ColdBox Namespace

This namespace is a combination of namespaces that are only active when used within a ColdBox application:

| DSL | Description |
| :--- | :--- |
| coldbox | Get the coldbox controller reference |
| coldbox:flash | Get a reference to the application's flash scope object |
| coldbox:setting:{setting} | Get the coldbox application _{setting}_ setting and inject it |
| coldbox:fwSetting:{setting} | Get a ColdBox setting _{setting}_ and inject it |
| coldbox:setting:{setting}@{module} | Get the coldbox application _{setting}_ from the _{module}_ and inject it |
| coldbox:datasource:{alias} | Get a new datasource struct according to _{alias}_ |
| coldbox:loaderService | Get a reference to the loader service |
| coldbox:requestService | Get a reference to the request service |
| coldbox:handlerService | Get a reference to the handler service |
| coldbox:interceptorService | Get a reference to the interceptor service |
| coldbox:moduleService | Get a reference to the ColdBox Module Service |
| coldbox:renderer | Get the ColdBox rendering engine reference |
| coldbox:dataMarshaller | Get the ColdBox data marshalling reference |
| coldbox:interceptor:{name} | Get a reference of a named interceptor _{name}_ |
| coldbox:configSettings | Get the application's configuration structure |
| coldbox:fwSettings | Get the framework's configuration structure |
| coldbox:fwSetting:{setting} | Get a setting from the ColdBox settings instead of the Application settings |
| coldbox:moduleSettings:{module} | Inject the entire _{module}_ settings structure |
| coldbox:moduleConfig:{module} | Inject the entire _{module}_ configurations structure |

```javascript
// some examples
property name="moduleService" inject="coldbox:moduleService";
property name="producer" inject="coldbox:interceptor:MessageProducer";
property name="appPath" inject="coldbox:fwSetting:ApplicationPath";
```

