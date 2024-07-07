Dashboards are proven and effective ways to portray our data. AWS has also got a product that can provide a dashboard from the data hosted in its S3 bucket. I followed Lucy Wang (@techwithlucy is her youtube channel) to learn about this fantastic service from AWS.

![Data vis diagram ](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/b1f7c55a-a6ab-404a-b3a0-cd6fb5b2b5ae)

The first step in the project is to extract a dataset for the dashboard. Also, a manifest file is required for the project in order to link to the data stored in the S3 bucket and create the QuickSight dashboard.

This project is straightforward and fairly easy to complete. Follow the below steps and you can understand how to build the dashboard:

Step 1: Navigate to the S3 service in the AWS console (You can either search this service from the "Search bar" or if you have used this service previously, it will appear under the "Recently Visited" tab.)

![1679318885819](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/5eb9a36b-d935-4f01-bee0-d5df979f81f0)

Step 2: Create a bucket with a unique name. I created one using the "Create Bucket" option and then with the name "quicksightsdemobucket1".

![1679319167749](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/f07fa14c-3559-432e-88f2-531a58deb809)

![Step 1 Edited](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/721eb9f1-ca57-4040-bf0c-bf4d7b745ea9)

• While creating the bucket, make sure to enable the "ACLs enabled" option.

Step 3: Uncheck the "Block All Public Access". Agree to the terms and conditions by checking the "I acknowledge ...." box under the block all public access setting.

![1679319475046](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/acf43e8e-2657-4102-bcf2-1d132a31fa44)

Step 4: Click on the "Create bucket" option to create the bucket.

![1679319926131](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/2fb5f613-19ff-4daa-9600-fa7366da33c6)

• If the bucket is created without issues, it will appear on the S3 console as shown below. Else, it will point you to the error point and we can modify the same.

![Edited Step 6](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/d383f7b9-03e9-4a72-ab34-798b573754e4)

Step 5: Click on the bucket created and it takes you to the next step where you can now add files.

![1679321239942](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/fec024f8-efec-47d0-ae80-e23c3fb52e85)

![1679321251513](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/a1854371-3bef-470b-be31-4dd8607d4f9a)

• Once the objects are added, it will show the successful message as below

![1679321347449](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/a89c4b8f-01ef-4667-a009-f3e8937ec57f)

Step 6: Create a manifest file with the data shown and the bucket name and data file detail and add this manifest.json file into the S3 bucket.

![1679324028856](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/cbafd4a6-e88f-4ef7-94a1-4150e1bf408e)

![Edited Step 7](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/b0678d81-655b-447a-b290-75562cb318e2)

Step 7:  Navigate to the QuickSight service in the AWS console

![Step for Quick sitght ](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/7394f9fa-31c4-4e5d-8418-6423910aa698)

• Once we click the QuickSight service, it takes us to the new page where it asks us to signup to use the service:

![Step 10](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/133cf27f-4415-415a-a80d-b527f5493fef)

• Once you are on QuickSight 

Step 8: Navigate to the "Datasets" option on the left-hand side of the screen

![Step 8 Edited](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/2ba3bf75-68e5-4faa-9049-d355ee057959)

Step 9: Now select the New Dataset option on the top right

![Step 9 Edited](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/9b2a17dd-cca2-4177-8cba-0b9a7f26e513)

Step 10: From the list, select S3 since we have hosted the dataset and the manifest file on the S3 bucket

![Step 10 Edited ](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/1e90ed23-e68f-4145-aa6c-bcd03d998156)

Step 11: Navigate to the manifest.json file in the S3 bucket created and copy the object URL

![Step 11 Edited ](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/a280f303-a7cf-4f96-8f3c-5ba95b9329a2)

Step 12: Navigate to the quicksight page where you have the popup for the datasource open, and paste it in the "Upload Manifest file" section and click on "Connect".

![Step 12 Edited ](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/7887abc7-7d2c-4f58-a5b6-f7de245e5867)

Step 13: Now click on "Visualize" to get your dashboard ready.

![Step 13 Edited ](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/37126113-bfe1-45dd-86af-d9e944fd4c02)

Step 14: From the list on the left, you can always do a drag-and-drop to create your visualizations. 

![1679327049282](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/20e0db21-7cc2-42a5-8617-4a0733b7f892)

• So this is how a sample dataset dashboard looks like:

![1679327165565](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/1268f386-2952-4f57-a430-8a723e934217)

• You can now use the dropdown to do some sorting work for the arrangement as needed and the options on the right for activities like saving the dashboard etc.

Most Popular Brands Chart:

![Most Popular Brands ](https://github.com/Blank-Brain-Check/AWS_Projects/assets/115382592/12efda17-5860-40eb-b2d3-60b47c6ef7d4)
