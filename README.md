# EHT Mayan EDMS deployment Repo

This repo is the deployment repo for the EHT instance of [MAYAN-EDMS](https://mayan-edms.com/).

    kubectl apply              \
    	    -f mb-secret.yaml  \
    	    -f db-secret.yaml  \
    	    -f bridge.yaml     \
    	    -f redis.yaml      \
    	    -f postgresql.yaml \
    	    -f mayan.yaml      \
    	    -f revsys.yaml
