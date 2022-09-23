1. Get list of installed operators by passing namespace 
    $oc get clusterserviceversion -n $namespace
    #or
    $oc get csv -n $namespace
    e.g $oc get clusterserviceversion -n openshift-marketplace
    
2. Get list catalog
  $oc get catalogsource -n $namespace
  e.g oc get catalogsource -n openshift-marketplace
   
3. To delete catalog
  $oc delete catalogsource/$catalog-source-name -n $namespace
  e.g $oc delete catalogsource/custom-operators -n openshift-marketplace

4. To check the catalog pods 
  oc get pods -n $namespace
  oc get pods -n openshift-marketplace
