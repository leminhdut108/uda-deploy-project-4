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

My config in circleci:

AWS_ACCESS_KEY_ID : AKIA2IBQLTCZ7R2YEXP6
AWS_BUCKET : minhhl2-bucket
AWS_DEFAULT_REGION : us-east-1
AWS_PROFILE : default
AWS_REGION : us-east-1
AWS_SECRET_ACCESS_KEY : tXmNOkEMdzPcUFI7deNJzBg1Cg0aYhQibexHkiS9


JWT_SECRET : minhhl2_secret
POSTGRES_HOST : database-1.ck3uod918mcw.us-east-1.rds.amazonaws.com
POSTGRES_DB : postgres
POSTGRES_PASSWORD : hocmai1234
POSTGRES_USERNAME : postgres

export POSTGRES_USERNAME=postgres
export POSTGRES_PASSWORD=postgres
export POSTGRES_HOST=udagramdb.cpmbomf1vmkr.us-east-1.rds.amazonaws.com
export POSTGRES_DB=postgres
export AWS_BUCKET=arn:aws:s3:::udagram-fe
export AWS_REGION=us-east-1
export AWS_PROFILE=default
export JWT_SECRET=hello
export URL=http://localhost:8080