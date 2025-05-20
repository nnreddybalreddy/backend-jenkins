@Library('jenkins-shared-library') _

def configMap=[
    type: "nodejsEKS",
    component: "backend",
    project: "expense"
]

// pipelineDecission.decidePipeline(configMap)

if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    pipelineDecission.decidePipeline(configMap)
}
else{
    echo "Proceed with CR or NON-PROD pipeline"
}