# web-page-db-get

In this task we will have a ESP32 with dht11 sensor (temperature & humidity sensor). <br>
we will read the temperature and humidity values and send it to **MYSQL** database, then we will get data from the database
and display the values to a website.<br>
**Note:** we can collect any type of data from any sensor and send it to the database.

### Pre-requisites:

To be able to send and get data from MYSQL database we have to install MYSQL database, you can use [XAMPP](https://www.apachefriends.org/) which i an open-source cross-platform web server.

### Explanation Walkthrough:

1. After installing **XAMPP** create a folder named "sensors" in xampp path *xampp>htdocs*

2. Copy the two files in Task3, **insert_temp.php** and **getSensorValues.php** to sensors folder

3. connect dht sensor to the ESP32 like this circut ![dht11 circut](https://i0.wp.com/randomnerdtutorials.com/wp-content/uploads/2019/04/dht_esp32_bb.png?w=714&quality=100&strip=all&ssl=1)

**Note:** use can use any sensor you would like.

4. Before uploading the code **DHT_MYSQL.ino** in Task3 folder, make sure to change the **ssid** and **password** to your WiFi

5. In **phpMyAdmin**, create a database named "esp32", then create a table named "dht" with values 

6. Now power ON the ESP32 and use the **index.html** and **app.css** files in *Task3* to test it.

7. Let the ESP32 run for few minutes to send data to MYSQL database, and as you can see database now have temperature and humidity data

8. the website should GET these data from the database and display it (display last added row) 

