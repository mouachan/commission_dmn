# commission_dmn

Web UI editor : https://kiegroup.github.io/kogito-online-staging/dmn-runner/#/editor/dmn
Bug cannot add values to a list from the generated runtime form tester : https://issues.redhat.com/browse/KOGITO-5111

Install rhpam operator from OperatorHub and create a Business Central instance from Openshift Operator Console :
```yaml
apiVersion: app.kiegroup.org/v2
kind: KieApp
metadata:
name: my-decision-svc-design-time
spec:
environment: rhdm-authoring
commonConfig:
adminUser: dmAdmin
adminPassword: dmAdmin
```
Swagger URL : https://my-decision-svc-design-time-kieserver-commisionnement.apps.cluster-10cf.10cf.sandbox1049.opentlc.com/docs/#/DMN%20models/getModels


ContainerId : commissionnement_1.0.0-SNAPSHOT
JSON Payload : 
```json
{
"model-namespace": "https://kiegroup.org/dmn/_7E972D37-8F93-492C-B297-BAECE5AC7838",
"model-name": "convention_1",
"dmn-context" : {
       "taux interet dossier":25,
       "type vehicule":"VO",
       "production" : 1000, 
       "taux interet marche":18,
       "Durree initiale financement" : 15, 
       "dossier annule resilie ou impaye" : false, 
       "type apporteur": "VD",
       "prestations" : ["GVA"],
       "duree initiale financement": 26,
       "type financement":"CREDIT_CLASSIQUE"
   }
}
```
