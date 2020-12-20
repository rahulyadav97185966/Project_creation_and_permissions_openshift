24  oc new-project farm --description="This is Openshift v3.5"
   25  oc projects
   26  oc default
   27  oc new-project sample --description="This is Openshift v3.5"
   28  oc new-project ditto --description="This is Openshift v3.5"
   29  oc new-project common --description="This is Openshift v3.5"
   30  oc new-project fedora --description="This is Openshift v3.5"
   33  oc adm policy add-cluster-role-to-user harry admin farm
   34  oc adm policy add-cluster-role-to-user harry admin sample
   35  oc adm policy add-cluster-role-to-user sagar edit ditto
   36  oc adm policy add-cluster-role-to-user sagar edit common
   37  oc adm policy add-cluster-role-to-user sagar admin fedora
   38  oc adm policy add-cluster-role-to-user harry view common
