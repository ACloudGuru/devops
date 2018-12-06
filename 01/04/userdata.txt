#!/bin/bash
sudo apt-get update -y
sudo apt-get install ruby -y
sudo apt-get install wget -y
cd /home/ubuntu
wget https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
chmod +x ./install
sudo ./install auto
service codedeploy-agent start
rm install
