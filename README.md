# my-docker-project
Steps to run the yml file:\n
 1-Install docker compose using cmd "yum install docker-compose"
 2-start docker services using cmd "systemctl start docker"
 3-Save the yml file in a new directory , enter the directory and run the yml file
      "mkdir /newdir
       cd /newdir
       docker-compose up"
  These steps will lead to a process where system will download the required image of container and run it. 
  This project help us to moniter and manage all the containers running in the host and we can see it through a web app
  Web app can be accessed using the port 4040 or 
  link:http://localhost:4040/
  And also we can access it in LAN using the ip of our host and accessing port 4040 of that ip
