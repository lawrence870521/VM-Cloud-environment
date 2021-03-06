AWS EC2 tutorial 
===
- [Create a Free Account](#account)
- [Create an EC2 instance](#EC2)
- [PuTTY Utilities](#putty)
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

### <a name="putty"> PuTTY Utilities </a>
1. Install **[PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)** on your local computer.

2. Click **Search**, key-in **PuTTYgen** and open it.
  
![](https://i.imgur.com/OXQ694l.jpg)

3. Under **Type of key to generate**, choose **RSA**.

![](https://i.imgur.com/RsxsIe7.png)

4. First, choose **Load** and display files of all types. Second, select your **.pem** file and open it.

![](https://i.imgur.com/SkoWwbE.jpg)

5. Save private key. **PuTTYgen** will display a warning about saving the key without a passphrase.

![](https://i.imgur.com/1eNZ73x.jpg)


### <a name="instance"> Connect to instance </a>
1. Start **PuTTY**.
2. In the **Category** pane, choose **Session** and complete the following fields:
    
    * To connect using your instance's public DNS      name, enter ***my-instance-user-name@my-instance-public-dns-name***. You can copy Host name on **EC2 Mangement Console** and click **Connect**.
    
    ![](https://i.imgur.com/sYD11Ts.jpg)
    
    ![](https://i.imgur.com/1Pih2uX.png)
    
    * Ensure the the **Port** value is 22.
3. (Optional) Avoid disconnecting from your instance due to session inactivity, you can configure **PuTTY** to automatically send "keepalive" data at regular intervals to keep the session active. In the **Category** pane, choose **Connection**, and then enter the required interval in the **Seconds between keepalives** fields.

![](https://i.imgur.com/CawCxN6.png)

4. In the **Category** pane, expand **Connection**, expand **SSH**, and the choose **Auth**. Complete the following:

    * Choose **Browse**.
    * Select the ***.ppk*** file that your generated for your key pair and choose **Save**.
    * Choose **Open**.

    ![](https://i.imgur.com/1h0PrQS.png)

5. Now, we can remote our VM.











   
    


