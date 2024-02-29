# How to Install Python 3.12 on Amazon Linux 2

## Step 1 – Update System
```
sudo yum update -y

sudo yum groupinstall "Development Tools" -y

sudo yum erase openssl-devel -y

sudo yum install openssl11 openssl11-devel  libffi-devel bzip2-devel wget 
```

## Step 2 – Download Python 3.12 on Amazon aws Linux 
```
wget https://www.python.org/ftp/python/3.12.0/Python-3.12.0.tgz 
tar xzf Python-3.12.0.tgz 
```

## Step 3 – Install Python 3.12 on Amazon aws Linux 2
```
cd Python-3.12.0
sudo ./configure --enable-optimizations 
sudo make altinstall        //compile
```

## Step 4 – Verify Python Installation
```
python3 -V
```
** Or Run the install-python3.12 bash script **

## Note: Before running the script make the file as LF
