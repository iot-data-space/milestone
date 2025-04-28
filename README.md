# MILESTONE Data Space
A FIWARE-based data space for sharing IoT data. The data space was developed
in the context of the MILESTONE project.

## Authors
* Nikos Fotiou, [ExcID](https://excid.io/)
* Spyros Chadoulos, [Plegma Labs](https://pleg.ma/)

## Execution 
Execute the following docker compose command

```
docker-compose -f milestone.yml up --build
```

## Contents
The repository includes a data space protected by a Policy Enforcement Point (PEP).
The PEP allows requests that include in their header a JWT access token, signed by
a trusted Identity Provider. In this example, the public key of the provider is included
in the configuration of the PEP proxy.

Additionally, the examples folder includes scripts for generating the such a JWT
access token, as well as for interacting with the data space using the ETSI NGSI-LD
API. 

## Acknowledgements
The MILESTONE project has received funding by the TrialsNet open call under Grant 10109587
