# AWS-IoT-Basic-Codes
Basic codes for establishing Publish and Subscribe communication with AWS using Random value generator

Go to AWS IoT Core.
Create a Thing from manage menu ( don't click on get started option)
Create a Certificate
Click on created certificate.
Download Certificate files.
Keep them in your project folder.
click on download Root Ca link .
(skip this step if you download AmazonRootCA1.pem from here) On the new documentation tab of this url: https://docs.aws.amazon.com/iot/latest/developerguide/managing-device-certs.html
(skip this step if you download AmazonRootCA1.pem from here) click on Amazon Root CA 1.
(skip this step if you download AmazonRootCA1.pem from here) which will open this page  Url : https://www.amazontrust.com/repository/AmazonRootCA1.pem
(skip this step if you download AmazonRootCA1.pem from here) Copy the Whole Content
(skip this step if you download AmazonRootCA1.pem from here) Create a New file in your project folder with Name 'AmazonRootCA.pem'
(skip this step if you download AmazonRootCA1.pem from here) Paste the content in it and save.
Activate Certificate
Go back to Manage>Things menu.
Click on Secure > Policies.
Click on Create Button.
Create A security policy with a Name  and in Action IoT:* and in Resouce *   , Chcek Allow. Click Create
Go to certificates . Click on your certificate.
From Action Menu Attach policy with Certificate. ( choose the latest one you Just Created. )
Similarly from action menu Attach thing  with the certificate ( choose the latest one you Just Created.)
Make sure your system has Pyhton3 ,Paho-mqtt ( pip3 install paho-mqtt ), pyOpenssl  (pip3 install pyOpenSSL) and AWSPythonIoTSDK ( pip3 install AWSIoTPythonSDK
) installed in it.
Put Python program files in your project folder where certificates are already.
Replace Awshost  (Manage> things> open your thing > interact >copy endpoint ), clientid (your thing name),thingname (your thing name),root certificate path (AmazonRootCA1.pem), certificate path (Your downloded thing certificate file name), private key path (Your downloded thing private key file name)and your topic name ( as your choice) in the file with your credentials from Aws console and downloaded file name
run with sudo python3 prefix and check in IoT Core Test option using the topic name.
