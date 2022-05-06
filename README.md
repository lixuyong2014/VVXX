# Apollo has unauthorized access vulnerability, allowing ordinary users to view pages that can only be displayed by super administrators.
This is the default super admin account page，apollo/admin
![image](https://user-images.githubusercontent.com/83060696/167172981-dddbd59c-1548-4a5d-9f96-354ee4e06690.png)
Next we create an account
![image](https://user-images.githubusercontent.com/83060696/167173020-d764097f-a922-491d-93dc-11008f9a2249.png)
![image](https://user-images.githubusercontent.com/83060696/167173076-f3109e46-c545-474a-b18a-2c2524eac9d7.png)
Then log in with the account you just created
![image](https://user-images.githubusercontent.com/83060696/167173092-232da5fa-6bfe-46e1-9bae-5b7791c305d2.png)
Then we press F5 to refresh and capture packets
![image](https://user-images.githubusercontent.com/83060696/167173131-33eb5b9d-4b00-48c3-beb3-070f2f2f93e8.png)
Change this response packet userId to super administrator apollo，then forward
![image](https://user-images.githubusercontent.com/83060696/167173147-963973ed-e95d-412d-8ae9-f47b06494aea.png)
Modify the hasPermission attribute of this response packet to true
![image](https://user-images.githubusercontent.com/83060696/167173109-fea5dbd0-6a38-4c4c-b280-65ea7dade394.png)
Then this response packet appears again, continue to modify
continue to pack
![image](https://user-images.githubusercontent.com/83060696/167173155-cb4a9837-e396-4430-b8b0-43a1590f3ee0.png)
Then we can see the menu bar that only super administrators can see
,We can use the same method to get unauthorized access to the User Management page and other pages
