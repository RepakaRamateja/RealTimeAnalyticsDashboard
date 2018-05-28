# RealTimeAnalyticsDashboard

</br>

This project is part of course Specialization in Big Data with Hadoop & Spark by CLOUD X LAB.

Taught By : Sandeep Giri  Abhinav Singh  Rohit Gupta  Jatin Shah



    Overview:

    Built a real-time analytics dashboard to visualize the number of orders getting shipped every minute to improve the performance of their logistics of a ecommerce comapany.



<br>

    Technologies Used:

    Apache Spark 

    Python

    Kafka 

    Node.js

   	Socket.IO  

   	Highcharts 

   	CloudxLab 


</br>

</br>

    Architecture:

![alt text](https://github.com/RepakaRamateja/RealTimeAnalyticsDashboard/blob/master/architecture.png)

</br>

 Step1:

 Since we do not have an online e-commerce portal in place, we took a dataset containing CSV files for simulating a ecommerce portal.

 Step2:

 Push Dataset to Kafka

 Step3:

 Spark Streaming and Kafka integration

 Step4:

 As soon as a new message is available in the one minute Kafka topic, node process consumes it. The consumed message then gets emitted to the web browser via Socket.IO

 Step5:

 As soon as socket.io-client in the web browser receives a new ‘message’ event, data in the event gets processed. If the order status is “shipped” in the received data, it gets added to HighCharts series and gets displayed on the browser.

 Step6:

 Run Node.js server  and then access dashboard from browser 


</br>

click the below link to see more information about this project 

https://cloudxlab.com/blog/real-time-analytics-dashboard-with-apache-spark-kafka/

 
</br>

