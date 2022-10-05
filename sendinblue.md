# Send in blue for custom email domain

- Where did I find sendinblue? [Click here](https://www.wpoven.com/blog/free-smtp-servers-sending-emails/)

- Adding Domain: https://youtu.be/b1a6lN2UwCY

- **Api looks cool as well:**

![image](https://user-images.githubusercontent.com/31458531/194028795-b37ca069-cc3c-43c2-9b32-e43b8856afb3.png)

- Checking if you are receiving request on pi server?

```bash
telnet mailer.sahilrajput.ml 25
# To close the request use: ctrl+] quit 
```

- How do I create a new user `hi` so that I can receive mails at `hi@sahilrajput.ml` ?

  [Source1](https://stackoverflow.com/a/29737950/10012446), [Source2](https://www.serverwatch.com/guides/adding-users-and-aliases-for-postfix/)

  tldr; Simply add a new user to linux system and postfix will handle rest. yo!!

- How do i see mails for each user, mails received for each user?

  Simplest way is to use alias: `pf.cdMail` which is aliased to `cd /var/spool/mail` and it'll show you all the ***emai-files*** for all users.
  
  Elegant way is to login to each desired user using thunderbird, and thus it'll be more convenient seeing messages in better ui. BUT YOU'LL still *NOT* be able to send emails bcoz IPS blocks your outbound 25 port and they charge 590RS./month for the static ip (they only allow opening outbound port 25 for static ips). FUCK THEM.

- Domain Settings for vercel (and freenom: domain nameservered to vercel dns) for receiving the initial verification email when adding `sendinblue` smtp email to gmail (required to do for once only and then you can close your postfix server for sure).

  ![image](https://user-images.githubusercontent.com/31458531/194108102-70c451c3-4d36-4f11-be74-f076f0f285e3.png)

  ![image](https://user-images.githubusercontent.com/31458531/194104111-9b169597-1ec0-4f9a-b8a3-5cebac230430.png)

- Add another email to gmail:

  In sendinblue dashboard, you need to add email as:

  ![image](https://user-images.githubusercontent.com/31458531/194110591-5ead8858-f444-49ef-8528-dd5229f892f4.png)

  So below how we set the add my email address (optionaly you can set it as default so by sending any email from gmail would select hi@sahilrajput.ml by default).
  
  ![image](https://user-images.githubusercontent.com/31458531/194106620-ac1a144d-860f-429a-b846-61c2040bf0b0.png)

  ![image](https://user-images.githubusercontent.com/31458531/194104636-20174c21-71f1-4a1f-8f8e-f6ba8d595f1f.png)

  ![image](https://user-images.githubusercontent.com/31458531/194105820-d2be39a6-a835-47db-9757-76b41bc1acc2.png)
