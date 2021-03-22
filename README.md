# EHT Mayan EDMS deployment Repo

This repo is the deployment repo for the EHT instance of [MAYAN-EDMS](https://mayan-edms.com/).

For a production deployment, the system admin should first change the `password` fields in both "mb-secret.yaml" and "db-secret.yaml", make sure that these passwords are **NOT** committed to git and **NOT** published to the internet, and then run the following command:

    kubectl apply              \
    	    -f mb-secret.yaml  \
    	    -f db-secret.yaml  \
    	    -f bridge.yaml     \
    	    -f redis.yaml      \
    	    -f postgresql.yaml \
    	    -f mayan.yaml      \
    	    -f revsys.yaml
