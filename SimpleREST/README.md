1) Create a spring boot app.
2) Create a project jar file.
	-Do maven clean and install , then you will get automatica jar file in target folder.
3) Create docker file.
	-Right click on root of project and create fle with name Dockerfile.
	-Write instructions int it.
4) Open cmd and pass command 'wsl' to open docker.And give password.
5)Then to build docker iamge , first traverse o your project location by 'cd C:\Users\shruti\Documents\JAVA_LEARNING\SimpleREST'.
6) Pass command, 'docker build . -t rest-app' , here rest-app is my docker iamge name.
7) Now we can see our docker image by passing command 'docker images'
8) Now to run this docker image. We can pass 'docker run -p 8081:8081 rest-app'.
	NOTE: - Docker iamge build will be done from project's path but we can find or run our docker image from any path ,
		     Not needed to be in project's path to run our docker image.
:) Now our rest-api docker image is running, we can pass REST endpoint (i.e. 8081/rest) to check it on postman/browser.


TO RUN DOCKER:
1.write 'wsl' on cmd
2.enter password
3.cmd 'docker images'	=>wil retrun all images present 
4.cmd 'docker run -p <defaultPortNumber:defaultPortNumber> <image name>