# AWS CORE SKILLS BOOTCAMP


## 1. EC2 instance demo 

### Update Ubuntu
```ubuntu

sudo apt update

```


### verify that git is available 

```ubuntu

git -v

```

### Install Git
```ubuntu

sudo apt install git -y

```

### Clone the repo 

```ubuntu

git clone https://github.com/iam-deepakverma/AWS-core-skills-bootcamp.git

```

### check for the repo folder 

```ubuntu

ls

```


### change the directory 

```ubuntu

cd AWS-core-skills-bootcamp

```

### check the folder 

```ubuntu

ls

```

### install apache server 

```ubuntu

sudo apt install apache2 -y

```

### move our index.html file to server directory 

```ubuntu

sudo cp index.html /var/www/html/

```

### verify it by 

```ubuntu

ls /var/www/html/

```

### start the server 

```ubuntu

sudo systemctl start apache2

```

```ubuntu

sudo systemctl enable apache


```


### to stop the server 

```ubuntu

sudo systemctl stop apache2

```


## 2. S3 Bucket demo 

### bucket policy 
```ubuntu 

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicRead",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "<your bucket arn >/*"
    }
  ]
}

```