# AWS-IoT-Basic-Codes
Basic codes for establishing Publish and Subscribe communication with AWS using Random value generator

Go to AWS IoT Core.
Create a Thing from manage menu ( don't click on get started option)
Create a Certificate
Click on created certificate.
Download Certificate files and Root Ca files.
keep those in your project folder.
Click on Create Security Policy
Create A security policy with IoT:* and Resouce *
Attach the policy with Certificate
Attach the certificate with your registered things
Make sure your system has Pyhton3 , Openssl and AWSPythonIoTSDK installed in it.
Put Python program files in your project folder where certificates are already.
run  and check in IoT Core Test option using the topic name.
