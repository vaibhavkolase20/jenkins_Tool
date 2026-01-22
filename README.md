  # Install jenkins
  # update your machine
      sudo apt update
      sudo apt upgrade -y
    
  # install java
      sudo apt install fontconfig openjdk-17-jre -y
  # java -version




---
  # Add Jenkins GPG Key

      curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
      /usr/share/keyrings/jenkins-keyring.asc > /dev/null


  # Add Jenkins Official Repository
      echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
      https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
      /etc/apt/sources.list.d/jenkins.list > /dev/null

  # Update your machune
      sudo apt-get update

  # install jenkins
      sudo apt-get install jenkins -y

  # Start Jenkins Service
      sudo systemctl start jenkins

  # Enable Jenkins to Start on System Boot
      sudo systemctl enable jenkins
      
  


  # jenkins runing on portnumber 8080 you attach this port number in your security group of ec2 instance
