# PITA Colab

This repository provides a Google Colab notebook implementation of PITA. It allows you to process vendor invoice PDFs directly in Colab and prepare them for Alma ingestion.

## Getting Started

Follow these steps to configure and run the notebook:

1. **Update credentials**  
   In `Amazon_Invoices_Processing_Notebook.ipynb` (Step Three), replace the placeholder values with your own:  
   - `MY_HOSTNAME` > your SFTP hostname  
   - `MY_USERNAME` > your SFTP username  

2. **Add your Alma RSA key as a Colab secret**  
   - Open the **Secrets** panel in Colab.  
   - Create a new secret with the following:  
     - **Name:** `ExL_sftp_is_rsa_file`  
     - **Value:** paste the contents of the `is_rsa` private key file you received from Alma.  

Once these are set, you can run the notebook end-to-end to deploy the PITA workflow in a Colab environment.
