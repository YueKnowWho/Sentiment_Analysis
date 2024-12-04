# Sentiment_Analysis
This project allows people to enter reviews and it will tell you if the review is a positive or negative review.

### Requirements
1. AWS CLI (https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

### How to run
1. Clone and cd into repository

```git clone https://github.com/YueKnowWho/Sentiment_Analysis.git && cd Sentiment_Analysis```

2. Run CloudFormation command using aws cli

```aws cloudformation deploy --template-file template.yaml --stack-name Sentiment-Analysis --capabilities CAPABILITY_NAMED_IAM```

3. In the AWS console, go to Cloudformation and search for `Sentiment-Analysis`

```https://console.aws.amazon.com/cloudformation/home```

4. Click on "Outputs" tab

5. Click on the "WebsiteURL" link. This should take you to the HTML website.

6. To view CloudWatch logs, go to the following link:

```https://console.aws.amazon.com/cloudwatch/home```

search for "/aws/lambda/Group11ReviewProcessor", and open the most recent Log stream


### How to delete
1. To delete all AWS resources created, run the following command:

```
aws cloudformation delete-stack --stack-name Sentiment-Analysis
```

2. To delete the CloudWatch logs:

```aws logs delete-log-group --log-group-name "/aws/lambda/Group11ReviewProcessor"```

```aws logs delete-log-group --log-group-name "/aws/lambda/Group11WebsiteLambdaFunction"```


-----

### Group 11 Members
* Anson Lu
* Jason Li
* Jonathan Yue
* Jeffrey Chan

Date: 12/4/2024