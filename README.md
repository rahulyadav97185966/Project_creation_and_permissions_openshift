        oc new-project farm --description="This is Openshift v3.5"
        oc projects
        oc default
        oc new-project sample --description="This is Openshift v3.5"
        oc new-project ditto --description="This is Openshift v3.5"
        oc new-project common --description="This is Openshift v3.5"
        oc new-project fedora --description="This is Openshift v3.5"
        oc adm policy add-cluster-role-to-user harry admin farm
        oc adm policy add-cluster-role-to-user harry admin sample
        oc adm policy add-cluster-role-to-user sagar edit ditto
        oc adm policy add-cluster-role-to-user sagar edit common
        oc adm policy add-cluster-role-to-user sagar admin fedora
        oc adm policy add-cluster-role-to-user harry view common
