<h2>Docker build:</h2>
<pre>>> docker build --tag study-sync:1.0 .</pre>
<h2>Docker Run:</h2>
<pre>>> docker run --env PORT=8080 --publish 8080:8080 --name ss -it study-sync:1.0 </pre>

<h2>Adding couple commands here:</h2>
If somehow end up executing `docker run` again, make sure to remove existing container or change the name of the container

<h2>Docker container list: </h2>
<pre>>> docker ps -a</pre>

<h2>Remove container: </h2>
<pre>>> docker rm ${CONTAINER_ID}</pre>
<pre>>> ${CONTAINER_ID} - would get that in the above step</pre>
or 
<h2>Change container name: </h2>
<pre> >> docker run --env PORT=8080 --publish 8080:8080 --name ${container_name} -it study-sync:1.0 </pre>
<pre>Note: ${container_name} replace your desired name </pre>
<h3>If you are running docker in AWS Ec2:</h3> make sure to add INBOUND RULE in ec2 instance with <b>custom tcp</b> and <b>port 8080</b>
