# Sentiment_Analysis
This project allows people to enter reviews and it will tell you if the review is a positive or negative review.

### Requirements
1. aws cli 

### How to run
1. Clone and cd into repository

```git clone https://github.com/YueKnowWho/Sentiment_Analysis.git && cd Sentiment_Analysis```

2. Run cloudformation command using aws cli

```aws cloudformation deploy --template-file template.yaml --stack-name Group11FinalProjectv2 --capabilities CAPABILITY_NAMED_IAM```

3. In the aws console, go to Cloudformation and search for `Group11FinalProjectv2`

4. Click on Outputs

5. Click on the WebsiteURL value. This should take you to the website.

### How to delete
1. ```aws cloudformation delete-stack --stack-name Group11FinalProjectv2```

### Group 11 Members
* Anson Lu
* Jason Li
* Jonathan Yue
* Jeffrey Chan