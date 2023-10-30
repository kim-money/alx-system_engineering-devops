0x0F-load_balancer

>>>>>>>>>>>>>>>

Load balancer
In this project i learnt how to setup a high availabilty infrastructure. A load balancer facilitates redundancy for the backend layer(web/app servers) but for a true high availabilty set up we need to have redundant load balancers as well. I also looked at the various algorithmns for load balancing and how they work. In the tasks i installed a HAproxy server and configured it to load balance 2 web servers.
Project Tasks
Task	Description
0. Double the number of webservers	In this first task you need to configure web-02 to be identical to web-01: Configure Nginx so that its HTTP response contains a custom header (on web-01 and web-02), The name of the custom HTTP header must be X-Served-By, The value of the custom HTTP header must be the hostname of the server Nginx is running on. Write 0-custom_http_response_header so that it configures a brand new Ubuntu machine to the requirements asked in this task
1. Install your load balancer	Install and configure HAproxy on your lb-01 server: Configure HAproxy so that it send traffic to web-01 and web-02, Distribute requests using a roundrobin algorithm, Make sure that HAproxy can be managed via an init script, Make sure that your servers are configured with the right hostnames: [STUDENT_ID]-web-01 and [STUDENT_ID]-web-02. If not, follow this tutorial, For your answer file, write a Bash script that configures a new Ubuntu machine to respect above requirements
2. Add a custom HTTP header with Puppet	Just as in task #0, we’d like you to automate the task of creating a custom HTTP header response, but with Puppet: The name of the custom HTTP header must be X-Served-By, The value of the custom HTTP header must be the hostname of the server Nginx is running on, Write 2-puppet_custom_http_response_header.pp so that it configures a brand new Ubuntu machine to the requirements asked in this task
