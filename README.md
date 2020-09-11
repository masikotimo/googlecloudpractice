Google Cloud Practice
========================

# Qwiklabs Screenshots 


**NB:** I have worked on 10 labs and each lab mentioned below links you to each of the screenshots required  saved in the google drive. 
 Together with 3 Translation tasks

## Course: Google Cloud Platform Fundamentals - Core Infrastructure

### Module: Getting Started with Google Cloud Platform

*   **[Getting Started with Cloud Marketplace](https://drive.google.com/file/d/1Nu6DkJpf1dOVXooBqg6l6tqO2kqX9WVb/view?usp=sharing).**

*   **[Getting Started with Compute Engine](https://drive.google.com/file/d/1A-kZxwri6iE0r_3VT2PiUMlnDLsZHMJx/view?usp=sharing).**


### Module: Containers in the Cloud

*   **[Getting Started with Kubernetes Engine:](https://drive.google.com/file/d/172YqsTtb7Cnw_FWr_LuMabHSIWQsura8/view?usp=sharing).**



### Module: Applications in the Cloud

*   **[Getting Started with App Engine:](https://drive.google.com/file/d/1kjy9ZLs-0hymCjwP5J0Gp02-vCGIyDzE/view?usp=sharing).**



## Course: Essential Google Cloud Infrastructure: Foundation

### Module: Introduction to Google Cloud

*   **[Console and Cloud Shell:](https://drive.google.com/file/d/1g7MSq2WuoFQG9m9PfTHHrqpptRYAA5_W/view?usp=sharing).**

*   **[Infrastructure Preview:](https://drive.google.com/file/d/1xLRIYIdhjSSuDJpXs6G1I3cPkr2ql7FF/view?usp=sharing).**

### Module: Virtual Networks

*   **[Implement Private Google Access and Cloud NAT:](https://drive.google.com/file/d/1mpAmCXgFhJiMqmCtj51OchNkNJ8gaT2M/view?usp=sharing).**


### Module: Virtual Machines

*   **[Creating Virtual Machines:](https://drive.google.com/file/d/1kVeEZO_dYsThH0OF2tmh0odE1A998wS_/view?usp=sharing).**

*   **[Working with Virtual Machines:](https://drive.google.com/file/d/1H-Tq07IbDMjJK6nQHWo4KFC44HOTUZfY/view?usp=sharing).**




## Course: Essential Google Cloud Infrastructure: Core Services

### Module: Cloud IAM

*   **[Cloud IAM:](https://drive.google.com/file/d/1eDPXmhWaco0duQ33ZzIrus6GLWZmBxOA/view?usp=sharing).**



# Translation

### Cloud IAM:

**Objectives**

*   **Use Cloud IAM to implement access control**
*   **Restrict access to specific features or resources**
*   **Use the Service Account User role**

**Steps**
1. gsutil ls gs://username1-bucketxx
2. For demoiam, SSH  connection.
3. gcloud compute instances list
4. gsutil cp gs://username1-bucketxx/sample.txt .
5. mv sample.txt sample2.txt
6. gsutil cp sample2.txt gs://username1-bucketxx



### Console and Cloud Shell

**Objectives**

*   **Get access to Google Cloud.**
*   **Create a Cloud Storage bucket using the Cloud Console.**
*   **Create a Cloud Storage bucket using Cloud Shell.**
*   **Become familiar with Cloud Shell features.**

**Steps**
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



### Implement Private Google Access and Cloud NAT

**Objectives**

*   **Configure a VM instance that doesn't have an external IP address.**
*   **Connect to a VM instance using an Identity-Aware Proxy (IAP) tunnel.**
*   **Enable Private Google Access on a subnet.**
*   **Configure a Cloud NAT gateway.**
*   **Verify access to public IP addresses of Google APIs and services and other connections to the internet.**

**Steps**
1. SSH to vm-internal to test the IAP tunnel <br/>
    gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap

2. To test the external connectivity of vm-internal, run the following command: <br/>
    ping -c 2 www.google.com

3. To return to your Cloud Shell instance, run the following command: <br/> 
    exit

4. Copy an image from a public Cloud Storage bucket to your own bucket. <br/>

    gsutil cp gs://cloud-training/gcpnet/private/access.svg gs://timbucketxx11

5. Access the image from your VM instance
    gsutil cp gs://timbucketxx11/*.svg . <br/>
    gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap <br/>
    gsutil cp gs://timbucketxx11/*.svg . <br/>
    gsutil cp gs://timbucketxx11/*.svg . <br/>

6. Try to update the VM instances <br/>
    sudo apt-get update <br/>
    gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap <br/>
    sudo apt-get update

7. Verify the Cloud NAT gateway <br/>
    sudo apt-get update

8. Configure and view logs with Cloud NAT Logging (Generating logs) <br/>
    gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap <br/>
    sudo apt-get update

