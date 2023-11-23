AWS Static Website Hosting on Amazon S3 with Custom Domain - Beginner's Guide
Welcome to the beginner's guide for hosting a static website on Amazon Simple Storage Service (S3) and using a custom domain with Amazon Route 53. This repository provides step-by-step instructions and screenshots to help you get started with hosting your static website and configuring a custom domain.

Prerequisites
Before you begin, ensure that you have the following:

An AWS account: If you don't have an AWS account, you can create one.
Basic understanding of static websites: Ensure your website consists of HTML, CSS, and other static assets.
A registered domain: Purchase a domain through a domain registrar like AWS Route 53 or any other registrar of your choice.
Getting Started
1. Log in to the AWS Management Console
Open your web browser and navigate to the AWS Management Console. Log in with your AWS account credentials.

2. Navigate to Amazon S3
In the AWS Management Console, search for "S3" or locate it under the "Storage" section. Click on "S3" to open the S3 console.

3. Create a New S3 Bucket
Click the "Create bucket" button.
Enter a unique and meaningful name for your bucket. Bucket names must be globally unique.
Choose the AWS Region for your bucket.
Click "Next" through the configuration options, leaving the default settings.
Review your settings and click "Create bucket."
4. Upload Your Website Content
Open the newly created bucket.
Click the "Upload" button.
Add your website files by either dragging them into the upload area or clicking "Add files."
Once all files are selected, click "Upload."
5. Configure the Bucket for Static Website Hosting
In the bucket properties, go to the "Static website hosting" card.
Choose "Use this bucket to host a website."
Set the index document (e.g., "index.html") and an optional error document.
Click "Save changes."
6. Create an Amazon Route 53 Hosted Zone
In the AWS Management Console, search for "Route 53" or locate it under the "Networking & Content Delivery" section.
Click on "Hosted zones" and then "Create hosted zone."
Enter your domain name and choose the default settings for the hosted zone.
Click "Create hosted zone."
7. Update DNS Records in Route 53
In your new hosted zone, click "Create Record Set."
For the name, enter your domain name (e.g., www.yourdomain.com).
Choose "Alias" as the type and select the S3 bucket you created as the target in the "Alias Target" field.
Click "Create."
8. Access Your Static Website with Custom Domain
After DNS propagation (which might take some time), you can access your static website using your custom domain.

Your website is now live at the custom domain you specified. You can share this URL for a more professional and branded experience.

Clean Up
To avoid incurring unnecessary charges:

Delete the objects in your S3 bucket.
Delete the S3 bucket itself.
Delete the hosted zone in Route 53.
Additional Resources
Amazon S3 Documentation
Amazon Route 53 Documentation
Hosting a Static Website Using Amazon S3
Congratulations! You have successfully hosted your static website on Amazon S3 with a custom domain using Amazon Route 53. If you have any questions or encounter issues, feel free to reach out for assistance. Happy hosting!