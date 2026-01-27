  # Install jenkins
  # update your machine
      sudo apt update
      sudo apt upgrade -y
    
  # install java
      sudo apt install fontconfig openjdk-21-jre
  # java -version
     java -version



---
  
  # install jenkins
  
      sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc \
      https://pkg.jenkins.io/debian-stable/jenkins.io-2026.key
      echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" \
     https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null
     sudo apt update
     sudo apt install jenkins

  # Start Jenkins Service
      sudo systemctl start jenkins

  # Enable Jenkins to Start on System Boot
      sudo systemctl enable jenkins
      
  


  # jenkins runing on portnumber 8080 you attach this port number in your security group of ec2 instance
