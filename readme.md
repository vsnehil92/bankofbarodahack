
## Solution

## Methodology
  1) Camera on the entrance of the bank identifying the unique faces to get the count of the customer.
  2) The exit and entrance time difference to calculate the average time spent by the customer for betterment of customer experience.
  3) Full body analysis of the customers through camera to check the weapons.
  4) Facial analysis of the customers and comparing it with previous records to check the number of times the customer visit the branch to rectify if he/she is a genuine customer.
## Architecture
  
![dfd drawio](https://user-images.githubusercontent.com/20948883/191318328-8c0d452d-5271-4f6e-85cf-6a694c9e0520.svg)

## Scalability
  1) Kubernetes pods running on demand to process the images and as the load increases so does the pods.
  2) Each branch can have seperate deployment yaml which can be scaled horizontly and can be scaled dynamically.
  3) Multiple services running on the images to process different data points from the image and then unify all the output to get an actual result.
  4) Common dashboard to monitor all the status.
  5) Models to be trained and pushed to s3. So that it can be pushed to any region on basis of domain and context of the client.
