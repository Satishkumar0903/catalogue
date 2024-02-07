#!groovy
@Library('robo_shop-shared-libraries') _

// responsibility to pass what type of application and component is this to pipeline deicssion

def configMap = [
    application: "nodejsVM",
    component: "catalogue"
]
if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    pipelineDecission.decidePipeline(configMap)
}
else{
    echo "This is PRODUCTION, deal with CR process"
}