# DevopsEngineer

~~![alt text](https://fsb.zobj.net/crop.php?r=MGX91JwQjDLfMqT0_k3GA6LwmXKHOl69nj3U_LYzlUllcx11e1XMkfbU8PjkHQcUBIBGjI_YSWhOhgvlDcoboPuzl43cfM7KQFehmhnwKOCZbHw6kzFP1gI0ed8YiXWvaovowmVn78GoiNpeTz7MB5WaXtKqS3ndcTPr4Ok1y6yTgF3rHZ1_yKeBxlOLEI-idg0whOpOqjWdq18U | width=100 )~~~


<img src="https://fsb.zobj.net/crop.php?r=MGX91JwQjDLfMqT0_k3GA6LwmXKHOl69nj3U_LYzlUllcx11e1XMkfbU8PjkHQcUBIBGjI_YSWhOhgvlDcoboPuzl43cfM7KQFehmhnwKOCZbHw6kzFP1gI0ed8YiXWvaovowmVn78GoiNpeTz7MB5WaXtKqS3ndcTPr4Ok1y6yTgF3rHZ1_yKeBxlOLEI-idg0whOpOqjWdq18U" width="100" height="100">


**Roles and Responsibloties**
- Devlopers will develop code and stores on version control,if they face any issue during merge conflicts ,my role is to help them 
-  My role is to make source code  build with build tools like maven ,if any errors on the console of CI tools(jenkins) ,required dependcies are added in POM.xml based    on error with the help of developers (I have worked on springboot application code )
-  Jenkins is used is as CI tool and geneated artifact from target folder is placed on JFROG 
-  My role is to use that docker image as image section of manifest kuberenetes and deploy to cloud either manually or using spinnakker tool.
-  My responsiliblities are to configure metric part like splunk ,grafana,prometheus and new relic agent 
-  For montoring deamon sets are deployed on each node ,for prometheus ,node exporter is used along with kube-state metrics to make prometheus understand metrics 
-  My reponsilibites also include building infra ,if needed like bastian host using terrraform modules which already exists
-  My role is also to configure servers using ansible and custom ami are build using packer provisioners



**Day to Day activities**
- helping the develop teams to upload code to git without merge conflicts
- Ceating new jenkins pipleines using libraries of jenkins exist
- creating infra needed like new ec2 instance or s3 bucket based on tickets assigned in sprint 
- configuring the servers using ansible like installing  zipping tool ,networking tools on all hosts 
-  making sure that all pods are running 
-  building new docker Images based on requirement using base Image




*Shell script*

```
#!/bin/bash
git status|tee log.txt >> /dev/null 2>&1
git add .|tee -a log.txt >> /dev/null 2>&1
echo Hello, Pls enter commit message
read varname
git commit -m "$varname"|tee -a log.txt >> /dev/null 2>&1
git push|tee -a log.txt >> /dev/null 2>&1
retVal=$?
if [ $retVal -ne 0 ]
then
    echo "Error"
else
    echo "@@@@@Be optimistic@@@@"
fi
exit $retVal

# generally enough >/dev/null see tee structure
#https://www.tecmint.com/delete-all-files-in-directory-except-one-few-file-extensions/
#rm -iv !(*.md)

```

[Refer to this blog reg ec2 instace start and stop](https://www.101daysofdevops.com/how-to-stop-start-ec2-instance-on-a-scheduled-basis-to-save-cost-by-using-boto3-and-lambda/)


| Devops Tools | Cloud  | Scripting |
| --- | --- | --- |
| Jenkins | AWS | python |
| Git| more | more |
| Terraform | more | more |
|Ansible | more | more |


*ALL THE BEST*
