# Challange-Lab
Perform Foundational Data AI,ML Task in Google cloud challange lab ....

# Task 1 : Run a simple Dataflow job
    bq mk lab
    gsutil cp gs://cloud-training/gsp323/lab.csv .
    cat lab.csv
    gsutil cp gs://cloud-training/gsp323/lab.schema .
    cat lab.schema

copy output it will have to be fill in when you create table in bigquery.

open Bigquery tab and in your project id create dataset <copy name> 
  after it in this dataset create table and table name is customers_698(copy yours from table row third)
  
  AFter it create bucket .
  
  search dataflow and create job **Text File cloud storage to bigquery should be in the BULK(batch)**

  # Task 2: Run a simple Dataproc job 
   after making cluster in the vm instances of this run hdfs whole coomand in ssh .
  then sumbit the job.
  
  
  # Task 3: Run a simple Dataprep Job 
   it is simple process 
  
  
  # Task 4: AI 
  **Important**
  
         
    gcloud iam service-accounts create my-natlang-sa \
      --display-name "my natural language service account"

    gcloud iam service-accounts keys create ~/key.json \
      --iam-account my-natlang-sa@${GOOGLE_CLOUD_PROJECT}.iam.gserviceaccount.com

    export GOOGLE_APPLICATION_CREDENTIALS="/home/$USER/key.json"
  

    gcloud auth activate-service-account my-natlang-sa@${GOOGLE_CLOUD_PROJECT}.iam.gserviceaccount.com --key-file=$GOOGLE_APPLICATION_CREDENTIALS

    gcloud ml language analyze-entities --content="Old Norse texts portray Odin as one-eyed and long-bearded, frequently wielding a spear named Gungnir and wearing a cloak and a broad hat." > result.json
  
      gcloud auth login --no-launch-browser

  
  **Create an API key and export as API_KEY variable**
  
      export API_KEY={Replace with API KEY}
  
  
  Done with lab do this carefully !!
  ALL the Best !!
