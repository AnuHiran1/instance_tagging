instancetagging


This scripts use the boto3 library to make AWS API calls. So if you don't have it, do:


    pip install boto3


csv-to-tags.py


This script will append tags to EC2 instances using a CSV file.


Example CSV file:



Instance-id	cluster	environment
i-xxxxxxxx	web	dev
i-xxxxxxxx	application	prod




Append tags to EC2 instances from a CSV file.
optional arguments:
-i     INPUT_FILE, --in INPUT_FILE  path to where the input file is located.


-r     AWS_REGION, --region AWS_REGION  AWS region to use.


Example usage:

python csv-to-tags.py -i tags.csv --region 'us-east-1'
