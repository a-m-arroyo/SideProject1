# CMPE 172 - Lab #3 Notes
## Part 1: Docker Compose
![Screenshot (554)](https://user-images.githubusercontent.com/13292772/223350177-865f0880-37d9-46fa-8525-61e735ca659b.png)


## Part 2: Gumball App and HA Proxy Load Balancer
#### When I load the page multiple times, the server host/IP interchanges between the IP addresses 172.18.0.3 and 172.18.0.4. These IP values are coming from the two gumball containers.
![Screenshot (545)](https://user-images.githubusercontent.com/13292772/223344192-cb291fe7-9045-4de0-8978-6c35696696d4.png)
![Screenshot (546)](https://user-images.githubusercontent.com/13292772/223344222-6f85e2fb-e205-4aa9-9a92-df8e7fdf2fd6.png)
#### When I try to put a quarter in to order a gumball, a whitelabel error page appears.
![Screenshot (547)](https://user-images.githubusercontent.com/13292772/223344243-2289f941-0ef9-4f07-a2ba-0f6a6c883f2c.png)
#### This error occurs when cookies are not enabled and causes the gumball page to jump between both gumball containers. By setting enable_cookies to true, the load balancer will route the page to a single gumball container and the page will work as intended.
![Screenshot (553)](https://user-images.githubusercontent.com/13292772/223346532-832b96cf-74b8-439d-b798-ddf39ada788a.png)
![Screenshot (552)](https://user-images.githubusercontent.com/13292772/223346526-9c218ec9-49a6-4db1-a207-0988b4ad6a36.png)
![Screenshot (555)](https://user-images.githubusercontent.com/13292772/223352570-b7d5cd8c-889f-4f86-be77-0e05a51afc35.png)
![Screenshot (556)](https://user-images.githubusercontent.com/13292772/223352582-9c738e2f-cce1-4359-84c5-fbf90bdf6cfe.png)


## Part 3: Jumpbox Testing
### Testing to see that the containers are up
#### Gumball 1
![Screenshot (542)](https://user-images.githubusercontent.com/13292772/223343206-ef3af52d-9e49-49ce-9e72-fd6b34d269fa.png)
#### Gumball 2
![Screenshot (541)](https://user-images.githubusercontent.com/13292772/223343259-92c87fc2-9a93-4da5-9e17-176c6eec05b1.png)
### Pinging the endpoints of the nodes behind the load balancer
#### Gumball 1
![Screenshot (543)](https://user-images.githubusercontent.com/13292772/223343284-2721c7cd-a807-4ab9-aa52-24993a94adce.png)
#### Gumball 2
![Screenshot (544)](https://user-images.githubusercontent.com/13292772/223343299-28bd11df-1217-4f1a-a5be-b3a3b87e1820.png)
