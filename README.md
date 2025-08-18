# docker-3


Docker Network Creation: The command docker network create petclinic-net successfully creates a new network named petclinic-net.
A container named spring1 and spring2 were started successfully, attached to the new network, and its internal port 8080 is mapped to the host's port 8081 and 8082.

![1](1.png)

we entered spring2 and made ifconfig 

![2](2.png)  
I entered spring1 and ping on the spring2 ip to see the outcomes .
The ping worked 

![3](3.png)  

The port 8081 worked for spring 1
![4](4.png)  

The port 8082 worked for spring 2

![5](5.png)  

Rerun spring1 and 2 with the all options in the petclinic-net network

![6](6.png)  

Run the new db ==> db1 and db2 and they have the same volume 

![16](16.png)

Run docker ps 

![7](7.png)  

Exec db1 
![9](9.png) 

Connect spring1 and spring2 with the db/clinic1 and clinc2 
![10](10.png)  

Create spring3 which have anothe network AND anothe db ---> db3 and have 8083 port
![11](11.png)  

Run docker ps
![12](12.png)  

Trying to connect spring3 with db1 and error happens
![13](13.png)  

connect spring3 with the other network which has db1 and db2 inside it 
![14](14.png) 

And connected sucessfully on port 8083
![15](15.png)




























