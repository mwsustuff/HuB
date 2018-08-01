web applications we can classfied two types
1. Model-1 or Mvc1
2. Model-11 or mvc2 or MVC

The struts2 framework is used to develop Mvc based applications.struts2 is the combination of webwork frmework of opensymphony and struts1

> Struts2=webwork+struts1

The struts2 provides supports to pojo based actions,validation support,ajax support,integration support to various frameworks such as Hibernate,spring,Tiles,
support to various results types such as FreeMaker,velocity,jsp....

### Interceptor
interceptor is used to perform operations such as validation,
exceptinhandling,internationalizaton,displaying intermediate result

### ValueStack
Valustack is simpliy a stack it contains application specific objects such as 
action objects and other model object

### ActionContext
The ActionContext is a container of objects in which action is execute.The values
stored in the ActionContext are unique per thread.So we dont need to make our action thread safe.
ActionInvocation
