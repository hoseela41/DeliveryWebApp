# DeliveryWebApp
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app). Front-end paprt is implemented by Javascript, CSS, html and React, backend is execued in Java environment, with assistance of libraries of Spring framework, Hibernate and Tomcat. Database used for storing users' input was established on MySQL instance of AWS RDB system.

The introduction of details could be seen in [slides](https://github.com/hoseela41/DeliveryWebApp/blob/main/images/LaiDelivery%201.0%20Demo.pdf).

The demo video could be seen at [demo link](https://www.youtube.com/watch?time_continue=1&v=04vbk0RKcxw&feature=emb_title)


## How to run the project to launch the website
1. Set the application server to be Tomcat > 9.0 versioin.
2. Front-end code is already packed in src/main/webapp folder, so the website will start automatically as running the package. 
3. The data has to be stored to [Amazon relational database service (RDS)](https://aws.amazon.com/rds/), please create your own RDS and import the data. Don't forget to change the url in the Application config file to connect to your own database.
4. Run Maven clean and install to import all dependencies we need.
5. Run Tomcat, wait for couple of minutes to have the project built.
6. Open your browser, enter http://localhost:8080/ to connect to the website, and you will see the home page

## What can we do on this website
1. At beginning, here's the welcome page that you could start our webapp or enter a tracking number to know where your pacakge is.![welcome](images/welcome.png)

2. At first page, please enter the account and passwod for log in. If it's your first time visiting the website, please hit *Register* button on top-right corner

2. Enter the information about your account, please note that error might pop-up if the content does not meet requirements.
![register](images/register.png)

3. After registration, you should be able to get back to home page, then enter your registered account and password. Hit the eyeball could show the password you entered.
![login](images/login.png)

4. Then there will be restarants to be selected, in this project, information of 3 restaurants were imported.
![restaurant](img/restaurant.png)

5. Select one of restaurant, the corresponding menu should appears.
![menu](img/burger.png)

6. You could hit the *plus* button to add food into cart, you should be able to see the button shows pending after hitting the object
![add](img/adding.png)

7. Hit the top-right *Cart* button, you should be able to see the food you ordered and how much should be paid. If you press checkout, then the cart will be cleared and information should show "successful payment was made".
![checkout](img/checkout.png)

8. Enjoy your food!