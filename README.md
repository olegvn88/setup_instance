#Jenkins job builder usage
> sudo pip install jenkins-job-builder
 
> sudo mkdir -p /etc/jenkins_jobs

> sudo vim /etc/jenkins_jobs/jenkins_jobs.ini

     [jenkins]
     query_plugins_info=False
     user=<user_name>
     password=<access_key>
     url=http://host:port

    jenkins-jobs test jobs
    jenkins-jobs update jobs
    jenkins-jobs delete \<jobName>
    jenkins-jobs delete-all -j
    jenkins-jobs delete-all -v

#Ansible usage
Go to aws_instance_setup and run:
 
> ansible-playbook jenkins.yaml -h hosts/jenkins.hosts