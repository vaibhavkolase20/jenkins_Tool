  # Install jenkins
      sudo apt update
    
      sudo apt install fontconfig openjdk-17-jre -y
  # java -version




---


      sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
       https://pkg.jenkins.io/debian/jenkins.io-2023.key

      echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
      https://pkg.jenkins.io/debian binary/ | sudo tee \
     /etc/apt/sources.list.d/jenkins.list > /dev/null

  # Update your machune
      sudo apt-get update

  # install jenkins
      sudo apt-get install jenkins -y


  # jenkins runing on portnumber 8080 you attach this port number in your security group of ec2 instance
