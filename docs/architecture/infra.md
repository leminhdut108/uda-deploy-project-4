AWS
RDS Postgres
The application server uses AWS RDS Postgres as database for storing and retrieving information.

Database URI: postgresql://postgres:hocmai1234@database-1.ck3uod918mcw.us-east-1.rds.amazonaws.com/postgres

Elastic Beanstalk
The application server is deployed on AWS Elastic Beanstalk service. The application is build, archived and uploaded to and S3 bucket from where Elastic Beanstalk extracts and runs the application on an endpoint.

## Application deployed link 
(The link below may be expired, please login again aws account)
- Udagram Frontend: http://minhhl2-bucket.s3-website-us-east-1.amazonaws.com/home
- Udagram API: http://minhhl2-eb.us-east-1.elasticbeanstalk.com/


### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```