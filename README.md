# api-lambda-s3
### 1. Create S3 Bucket & Enable Static Hosting
1. Log in to AWS S3.  
2. Create a bucket (e.g., `my-static-website`).  
3. Enable **Static website hosting** in bucket properties.  
4. Upload `index.html` and any other assets (CSS, JS, images).  
5. Make the bucket objects public (if needed for demo).  

### 2. Create Python Lambda Function
1. Go to AWS Lambda and click **Create Function**.  
2. Choose **Author from scratch** → Runtime: Python 3.x.

### 3. Create API Gateway
1.Go to API Gateway → REST API → Create API.
2.Create a Resource (e.g., /trigger).
3.Add a GET Method linked to your Lambda function.
4.Deploy the API to a stage (e.g., prod).
5.Copy the Invoke URL (endpoint).

### 4.Test Your Project
1.Open your S3 static website URL.
2.Trigger the Lambda function via API and check browser console for output.
