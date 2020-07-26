# StudentSIMS

URLs of APIs that have been hosted on Azure:

https://msa-phase11.azurewebsites.net/index.html



Database:

Address table:  
A student might have physical address and mailing address. So I decide to leave the thought one student can have two address or more.
![addressTable](https://user-images.githubusercontent.com/63832090/88175008-50fba680-cc79-11ea-96a4-7f00e85c60e7.PNG)

Student table:
![studentTable](https://user-images.githubusercontent.com/63832090/88176088-e0ee2000-cc7a-11ea-834b-80b25a6a0671.PNG)



API manipulate in Swagger UI:

'GET':
Using the 'GET' tab to retrieve data from data base at Address table. In ‘Server response’ show 200 under the ‘Code’ which means data transmit success and under ‘Details’ shows all Address table’s information. 
![Get Address result from Swagger UI](https://user-images.githubusercontent.com/63832090/88160839-53eb9c80-cc63-11ea-8cdf-7e213ef600ed.JPG)

Checking data on Address table, it is matched or not with displayed data on ‘GET’ tab. 
![Get Address check from dataBase](https://user-images.githubusercontent.com/63832090/88163074-408e0080-cc66-11ea-9266-766a406bf628.JPG)

'POST':
creating a new address for a student in Address table. 
![post](https://user-images.githubusercontent.com/63832090/88176918-1fd0a580-cc7c-11ea-98a8-c8c640dc78fa.PNG)

check the reesult in database.
![postDB](https://user-images.githubusercontent.com/63832090/88177238-a08fa180-cc7c-11ea-9b18-cd5640d8f0a3.PNG)

'GET': 
-get data with an address id.
![getwithid](https://user-images.githubusercontent.com/63832090/88177453-ffedb180-cc7c-11ea-98d2-a017d861dafc.PNG)

-check the result in database.
![getcheck](https://user-images.githubusercontent.com/63832090/88177637-565af000-cc7d-11ea-832e-9ec278c9a3e5.PNG)

'PUT':
-change an addree content.
![put](https://user-images.githubusercontent.com/63832090/88178101-f6b11480-cc7d-11ea-81bb-c7118b871927.PNG)

-check the change in database
![putdb](https://user-images.githubusercontent.com/63832090/88178241-34ae3880-cc7e-11ea-8522-9d09b7de03d5.PNG)

'DELETE':
-delete a record
![delete](https://user-images.githubusercontent.com/63832090/88178425-7b039780-cc7e-11ea-9f02-265bc139c6ba.PNG)

-check database
![deleteDB](https://user-images.githubusercontent.com/63832090/88178612-c6b64100-cc7e-11ea-894e-a9213e8395e6.PNG)


Assumtion:
-I try to modify C# code in AddressController.cs, in order to check if there is a ‘studentId’ exist in ‘Student’ table or not. However, I found before I create a ‘Controller’ I need to choose data content from AddressContext class. If I use Student context in AddressController.cs, I might mix up the data content between AddressController and StudentController. So, I decided to leave the constrained check. 
![C# assumption](https://user-images.githubusercontent.com/63832090/88166353-3c181680-cc6b-11ea-8779-61c4269a312e.JPG)


