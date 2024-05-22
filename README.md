# OT-MICROSERVICE Application Deployment

This project outlines the steps to set up and deploy the OT-MICROSERVICE application using Kubernetes pods.

## Step 1: Attendance Setup

### Option 1:
1. **Run MySQL in one pod**
   - Deploy a pod dedicated to MySQL.
2. **Run Attendance in one pod**
   - Deploy a separate pod for the Attendance application.
3. **Validation**
   - Ensure both MySQL and Attendance pods are running successfully and can communicate with each other.

### Option 2:
1. **Attendance & MySQL in one pod**
   - Deploy a single pod that contains both the MySQL database and the Attendance application.
2. **Validation**
   - Ensure the combined pod is running successfully and the Attendance application can access the MySQL database.

## Step 2: Additional Service Pods

1. **Run ES pod**
   - Deploy the ES (Elasticsearch) pod.
   - **Validation**: Ensure the ES pod is running successfully.
   
2. **Run Salary pod**
   - Deploy the Salary application pod.
   - **Ensure connectivity with ES pod**: Verify that the Salary pod can connect to the ES pod.
   - **Validation**: Confirm the Salary pod is operational and interacting correctly with the ES pod.

3. **Run Employee pod**
   - Deploy the Employee application pod.
   - **Ensure connectivity with ES pod**: Verify that the Employee pod can connect to the ES pod.
   - **Validation**: Confirm the Employee pod is operational and interacting correctly with the ES pod.

## Step 3: Frontend and Webserver Pods

1. **Run Frontend pod**
   - Deploy the Frontend application pod.
   - **Validation**: Ensure the Frontend pod is running successfully and is accessible.

2. **Run Webserver pod**
   - Deploy the Webserver pod.
   - **Validation**: Ensure the Webserver pod is running successfully and serving requests properly.

Follow the above steps to set up and validate each component of the OT-MICROSERVICE application. Ensure all pods are deployed, connected, and functioning as expected.
