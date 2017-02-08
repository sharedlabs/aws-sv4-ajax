# Polymer 2 \<aws-sv4-ajax\>

Iron-Ajax wrapper for signing requests for AWS private APIG endpoints using
Polymer 2


## Example

```
<aws-sv4-ajax
    id="ajax"
    api-endpoint="https://id.execute-api.eu-central-1.amazonaws.com/dev"
    path="apipath"
    method="get"
    params='{"foo":"bar"}'
    handle-as="json"
    region="eu-central-1"
    access-key-id="ASIAJUJT9T0JQ64J22RJ"
    secret-key="cTig+gy0LjjDfjcL3S1kd6w+8SFovw7MyDVLBSId"
    session-token="AgoGb3JpZ2luENT//////wEaDGV1LWNlbnRyYWwtMSKAAhz80TDA..."></aws-sv4-ajax>

```

```
this.$.ajax.generateRequest().then(response => {
  console.log(response);
});
```