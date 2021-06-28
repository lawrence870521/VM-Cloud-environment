AWS EC2 tutorial 
===
- [Create a Free Account](#account)
- [Create an EC2 instance](#EC2)
- [Connect to instance](#instance)



### <a name="account"> Create a Free Account </a>
1. [Sign up for AWS](https://portal.aws.amazon.com/billing/signup?refid=em_127222&redirect_url=https%3A%2F%2Faws.amazon.com%2Fregistration-confirmation#/start)
    **Notice:** In order to test the validity of this card, you need to enter your Credit or Debit card number. AWS will chrage $1 USD for testing and then refund it.
![](https://i.imgur.com/GVxR1jx.png)
2. Choose basic support.
![](https://i.imgur.com/kKN6Ru2.png)

### <a name="EC2"> Create an EC2 instance </a> 
1. Use the EC2.

![](https://i.imgur.com/qUidEhN.png)

2. Choose **Ubuntu server 20.04** and press Select.

![](https://i.imgur.com/Hrw4tzA.png)

3. Choose **t2.micro** and press **Review and Launch.**

![](https://i.imgur.com/qMtsT7M.png)

4. Check out the configuration and press **Launch.**

![](https://i.imgur.com/sGsP3sQ.png)

5. Now, you need to choose "Create a new key pair" and give a key pair name. Furthemore, do not forget to **download key pair**.

![](https://i.imgur.com/hKixF1G.png)

6. Finally, your instance was built successfully. Also, you can rename it.

![](https://i.imgur.com/LBReUUb.png)


### <a name="instance"> Connect to instance </a>
1. On your EC2 Mangement console, choose your instance and press **Connect**. 

![](https://i.imgur.com/SSurzZT.jpg)


2. We choose **SSH client** to connect our instances. You can see two commands which I circle it. We will use them next three steps.

![](https://i.imgur.com/CzAgDDQ.jpg)



3. First, open the terminal and change directory to where you store key pair. (For me, I store in **Downloads** folder.) 

![](https://i.imgur.com/OwCMdu5.png)
 
4. Key in **chmod 400 *yourkeypairname*.pem**. These command sets premissions so that, user/owner can read but can't write.
    **Notice:** remember to chanege *yourkeypairname* to your own.

![](https://i.imgur.com/oenu0Ka.png)

    
5. Finally, we key in ssh command to connect our VM. You can copy the whole command on Step2 to your terminal and execute it. 

![](https://i.imgur.com/Rl9VZPr.png)

6. Now, we can remote our VM.











   
    


