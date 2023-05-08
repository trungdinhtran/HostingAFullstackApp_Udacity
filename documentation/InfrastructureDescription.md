## Infrastructure Description

![Infrastructure](infrastructure.png)

### Summarize

When user access the link of AWS S3 to using the website. If any request of user need request to data. The front-end(AWS S3) will call back-end(ElasticBeanstalk) to get data. In this step back-end will call to database(RDS) to get data base on user request.

- **Elastic Beanstalk (API)URL**: http://udacity-api-dev.us-east-1.elasticbeanstalk.com/
- **S3 Bucket (Front-end) URL**: http://myawsbucket-953179853956.s3-website-us-east-1.amazonaws.com/