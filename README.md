# EHT Mayan EDMS deployment Repo

This repo is the deployment repo for the EHT instance of MAYAN-EDMS](https://mayan-edms.com/).

    kubectl apply                        \
	    -f bridge-networkpolicy.yaml \
    	    -f mb-secret.yaml            \
	    -f redis.yaml                \
	    -f db-secret.yaml            \
	    -f postgresql.yaml           \
	    -f mayan.yaml
