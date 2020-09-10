Google Cloud Practice
========================

# Qwiklabs Screenshots 

Course: Google Cloud Platform Fundamentals - Core Infrastructure

Module: Getting Started with Google Cloud Platform


### Getting Started with Cloud Marketplace:
[here](https://drive.google.com/file/d/1Nu6DkJpf1dOVXooBqg6l6tqO2kqX9WVb/view?usp=sharing){:target="_blank"}.




<br/>

### Getting Started with Compute Engine:
[here](https://drive.google.com/file/d/1A-kZxwri6iE0r_3VT2PiUMlnDLsZHMJx/view?usp=sharing).

<br/>


Module: Containers in the Cloud
### Getting Started with Kubernetes Engine:
[here](https://drive.google.com/file/d/172YqsTtb7Cnw_FWr_LuMabHSIWQsura8/view?usp=sharing).

<br/>



Module:Applications in the Cloud

### Getting Started with App Engine :
[here](https://drive.google.com/file/d/1kjy9ZLs-0hymCjwP5J0Gp02-vCGIyDzE/view?usp=sharing).

<br/>


Course: Essential Google Cloud Infrastructure: Foundation

Module: Introduction to Google Cloud


### Console and Cloud Shell:
[here](https://drive.google.com/file/d/1g7MSq2WuoFQG9m9PfTHHrqpptRYAA5_W/view?usp=sharing).

<br/>


### Infrastructure Preview:
[here](https://drive.google.com/file/d/1xLRIYIdhjSSuDJpXs6G1I3cPkr2ql7FF/view?usp=sharing).

<br/>


### Implement Private Google Access and Cloud NAT:
[here](https://drive.google.com/file/d/1mpAmCXgFhJiMqmCtj51OchNkNJ8gaT2M/view?usp=sharing).

<br/>


### Creating Virtual Machines:
[here](https://drive.google.com/file/d/1kVeEZO_dYsThH0OF2tmh0odE1A998wS_/view?usp=sharing).

<br/>


### Working with Virtual Machines:
[here](https://drive.google.com/file/d/1H-Tq07IbDMjJK6nQHWo4KFC44HOTUZfY/view?usp=sharing).

<br/>


Course: Essential Google Cloud Infrastructure: Core Services

Module: Cloud IAM


### Cloud IAM:
[here](https://drive.google.com/file/d/1eDPXmhWaco0duQ33ZzIrus6GLWZmBxOA/view?usp=sharing).

<br/>





Translation

### Cloud IAM:
1. gsutil ls gs://username1-bucketxx
2. For demoiam, SSH  connection.
3. gcloud compute instances list
4. gsutil cp gs://username1-bucketxx/sample.txt .
5. mv sample.txt sample2.txt
6. gsutil cp sample2.txt gs://username1-bucketxx



Console and Cloud Shell
1.  gsutil mb gs://timbucketxx2
2.  gsutil cp sample.txt gs://timbucketxx2
3.  gcloud compute regions list
4.  INFRACLASS_REGION=us-central1
5.  echo $INFRACLASS_REGION
6.  mkdir infraclass
7.  echo INFRACLASS_REGION=$INFRACLASS_REGION >> ~/infraclass/config
8.  INFRACLASS_PROJECT_ID=qwiklabs-gcp-04-19829e311f08
9.  echo INFRACLASS_PROJECT_ID=$INFRACLASS_PROJECT_ID >> ~/infraclass/config
10.  source infraclass/config   && echo $INFRACLASS_PROJECT_ID
11.  nano .profile
12.  source infraclass/config
13.  echo $INFRACLASS_PROJECT_ID



Implement Private Google Access and Cloud NAT

SSH to vm-internal to test the IAP tunnel
 gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap

To test the external connectivity of vm-internal, run the following command:
 ping -c 2 www.google.com

To return to your Cloud Shell instance, run the following command:
exit

Copy an image from a public Cloud Storage bucket to your own bucket.

gsutil cp gs://cloud-training/gcpnet/private/access.svg gs://timbucketxx11

Access the image from your VM instance
gsutil cp gs://timbucketxx11/*.svg .
gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap

gsutil cp gs://timbucketxx11/*.svg .
gsutil cp gs://[my_bucket]/*.svg .

Try to update the VM instances
sudo apt-get update
gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap

sudo apt-get update

Verify the Cloud NAT gateway
sudo apt-get update

Configure and view logs with Cloud NAT Logging
Generating logs
gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap
sudo apt-get update






*   **If using a phone,**



*  **If using an emulator,**

* **Optional: Install Watchman** <br/>




**NB:** WORK  **YES** check what 

