# helm-chart-streamlit

## kubectl
**kubectl** folder contains configuration in order to setup a streamlit app step by step on kubernetes (onyxia)
```
   kubectl apply -f deployment.yaml
   kubectl apply -f service.yaml
   kubectl apply -f ingress.yaml
```

## Helm chart
**streamlit-chart** folder contains a helm chart to run a streamlit app on onyxia
* To run it, adapt values.yaml.
  * host : if you want to display on a specific url name
  * image/repistory : with you own streamlit image
 
* To install the helm chart:
```
  helm install streamlit-chart ./streamlit-chart/.
```
