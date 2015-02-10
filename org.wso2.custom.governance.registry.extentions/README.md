==== Lifecycle Executor for API RXT ====

Custom Executor java class needs to implement the “Execution” interface that is provided by Governance Registry. Also you can find existing executor implementations under governance registry extension components.

When creating custom executor, you need to override two methods available in the “Execution” interface. They are init method and execute method. The "init" method is where parameters are defined. The "execute" method is where your custom execution related logic goes.

Example Usage

<execution forEvent="Promote" class="org.wso2.custom.governance.registry.executor.ApiStoreExecutorApiRxt">
	<parameter name="apim.endpoint" value="http://localhost:9764/" />
	<parameter name="apim.username" value="admin" />
	<parameter name="apim.password" value="admin" />
</execution> 

