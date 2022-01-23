## Load Balancer
1. It distributes the web traffic to available servers or backend servers
2. Internet facing LB has a DNS which further converted into IP address of IP address of LB.


<img width="500" height=300 alt="image" src="https://user-images.githubusercontent.com/84008107/150673407-c9fd56cc-983c-41bc-882c-d2befcf4859c.png">

## Elastic Load Balancer (ELB)
In Aws ELB are of 3 types

### Classic Load Balancer
1. A load balancer distributes incoming application traffic across multiple EC2 instances in multiple Availability Zones.
2. It supports HTTP,HTTPS,TCP,SSL

<img width="500" height=300 alt="image" src="https://user-images.githubusercontent.com/84008107/150675848-b0ccd0a5-74de-4634-81dc-e16b57c45919.png">

### Application Load Balancer (ALB)
1.  It functions at 7th layer (Application Layer) of the Open Systems Interconnection (OSI) model.
2.  It increases the availability of your application.
3.  It supports HTTP and HTTPS
4.  Support for Path conditions. You can configure rules for your listener that forward requests based on the URL in the request.
5.  <b>Listener</b> is a process that checks for connection requests, using the protocol and port that you configure. The rules that you define for a listener determine how the load balancer routes requests to its registered targets.
6.  <b>target group( Group of Ec2 instances)   </b> is used to route requests to one or more registered targets(Ec2 instance,IP,Lambda). When you create each listener rule, you specify a target group and conditions. When a rule condition is met, traffic is forwarded to the corresponding target group.

<b>Note:-</b> When Target type is IP then you can take the public IP addresses, you can use <b>ONLY</b> below CIDR Ranges
1. 10.0.0.0/8
2. 100.64.0.0/10
3. 172.16.0.0/12
4. 192.168.0.0/16

<img width="500" height=300 alt="image" src=https://user-images.githubusercontent.com/84008107/150674727-02377549-b1c3-4ce5-9c36-5fbe1e57bf43.png>




