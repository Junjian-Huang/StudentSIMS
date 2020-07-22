# StudentSIMS

Using the 'GET' tab to retrieve data from data base at Address table. In ‘Server response’ show 200 under the ‘Code’ which means data transmit success and under ‘Details’ shows all Address table’s information. 

![Get Address result from Swagger UI](https://user-images.githubusercontent.com/63832090/88160839-53eb9c80-cc63-11ea-8cdf-7e213ef600ed.JPG)


Checking data on Address table, it is matched or not with displayed data on ‘GET’ tab.

![Get Address check from dataBase](https://user-images.githubusercontent.com/63832090/88163074-408e0080-cc66-11ea-9266-766a406bf628.JPG)




I try to modify C# code in AddressController.cs, in order to check if there is a ‘studentId’ exist in ‘Student’ table or not. However, I found before I create a ‘Controller’ I need to choose data content from AddressContext class. If I use Student context in AddressController.cs, I might mix up the data content between AddressController and StudentController. So, I decided to leave the constrained check. 
![C# assumption](https://user-images.githubusercontent.com/63832090/88166353-3c181680-cc6b-11ea-8779-61c4269a312e.JPG)


