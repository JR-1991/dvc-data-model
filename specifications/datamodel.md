# ZnTrackNode

### MetaNode

- __nodes__
    - Type: Node
    - Multiple: True
    - Description:  Steps done in this workflow
- __parameters__
    - Type: Parameter
    - Multiple: True
    - Description: Parameters for this node
- __metrics__
    - Type: Metric
    - Multiple: True
    - Description: Metrics for this node
    
### Node 

- __step__
    - Type: int
    - Description: Step number for this workflow
    - Dataverse: pyDaRUS.Process.processing_steps.id
- __name__
    - Type: string
    - Description: Name of the step
    - Dataverse: pyDaRUS.Process.processing_steps.software
- __inputs__
    - Type: string
    - Multiple: True
    - Description: Parameters/files that are used as inputs
    - Dataverse: pyDaRUS.Process.processing_steps.input
- __dependencies__
    - Type: string
    - Multiple: true
    - Description: Script that is executed at runtime for this node
- __command__
    - Type: string
    - Description: Command used to execute this stage
    - Dataverse: pyDaRUS.Process.processing_steps.methods
    
### Parameter

- __name__
    - Type: string
    - Description: Name of the parameter
    - Dataverse: pyDaRUS.Process.method_parameters.name
- __value__
    - Type: float
    - Description: Value of the parameters
    - Dataverse: pyDaRUS.Process.method_parameters.value

    
### Metric

- __name__
    - Type: string
    - Description: Name of the parameter
- __value__
    - Type: float
    - Description: Value of the parameters
