# my-docker-project
Steps to run the yml file:</br> 
 1-Install docker compose using cmd "yum install docker-compose"</br>
 2-start docker services using cmd "systemctl start docker"</br>
 3-Save the yml file in a new directory , enter the directory and run the yml file</br>
      "mkdir /newdir</br> 
       cd /newdir</br>
       docker-compose up"</br>
  These steps will lead to a process where system will download the required image of container and run it.  
  This project help us to moniter and manage all the containers running in the host and we can see it through a web app 
  Web app can be accessed using the port 4040 or  
  link:http://localhost:4040/ 
  And also we can access only if we are in the same LAN as the host using the ip of our host and accessing port 4040 of that ip.</br>
  The above condition is applicable only if you have a private ip on your host system.
  
  <center><b>ABOUT THE PROJECT</b></br></center>
 The main idea behind docker is to run different modules or services individually in an isolated environment but still not taking up separate resources to execute and run as several services or modules can run on a single host using the host resources and sharing then among all the containers running at an instant. This makes dockers fast and more efficient.

 But imagine you have several containers running in your host at the same time, so now monitoring these containers is a bigger issue if you have to do this manually.
 To solve this issue I have used weave scope image to launch a weave scope service in a container in my system.
 After the setup you can access the weave UI using http://localhost:4040 and see a graphical view of all your containers along with their interlinking. Also you can enter the container just by clicking on the respective node shown on the screen and now can see the internal details about their configuration and services running on them and many other details.
 The web UI will get automatically updated whenever you launch a new docker or terminate any of them and reflect the same on the webpage.
 This makes monitoring containers very easy and handy.

 Here to test  my project I have launched two dockers working on the same host and internally dependent on each other as one of them uses the other for its services.
 WordPress is launched in one container which is using another SQL container for its database requirements.

 The whole project was doployed using docker-compose which helps you to launch several containers  and also interlink these containers by using a yaml file.
