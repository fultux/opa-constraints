# OPA contsraints CIS 1.23

## Description
Opa Gatekeeper Constraints for compliance to the CIS 1.23 profile.


## How to
Install OPA contstraint templates from the OPA-Gatekeeper library on your cluster.
See how to do it here: (https://github.com/open-policy-agent/gatekeeper-library)

The cluster-wide constraints are in the global-constraints folder. 
Before deploying them you must setup a value for YOUR-REPO in the file enforceImageRegistryGlobal.yaml. You must also set up the ID ranges inside the enforceUidGidGlobal.yaml file.

You can then apply the constraints to your cluster.

```
kubectly apply -f .
```

