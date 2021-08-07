# workflow-sdk

SDK for integrating workflow with logic codes

## Integrating with binaries

Import the package into the go code and pass the function to the `Start` function.

**NOTE:** input params to the handler are the params set in the workflow config when configuring this step.

```
package main

import (
    workflow "github.com/corepackge/workflow-sdk"
)

func handler(input interface{}) (string,error) {
    return "Hello, World"
}

func main(){
    workflow.Start(handler)
}
```
