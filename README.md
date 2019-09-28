# Restful-Web-Services
GIT Repository for cloud Homework2-Developed Restful Web Services to host weather information
The API provides the daily weather information of Cincinnati for the past 3 years.The data is in the form csv file.

<b><u>Environment Setup:</b></u>
<p><b>To install Django in AWS ubuntu instance follow these steps:</b>
<p>sudo apt-get install language-pack-en

enter - 'Y'

sudo locale-gen en_GB.UTF-8

sudo -i

apt update

apt install -y  python3-dev python3-setuptools python3-pip

pip3 install Django

pip3 install django-import-export ( not required since data is already in the db )

pip3 install djangorestframework


<b>Description:</b>
<p>The API services are generated for the following methods </p>

<p>GET - It provides a list of all the dates in the database of daily weather forecast</p>
<p>GET/{date}- It provides the details of the maximum and minimum temperature for the specified date</p>
<p>DELETE/{date} - It deletes the details of the maximum and minimum temperature for the specified date</p>
<p>Forecast/{date}- It returns the forecast for 5 days in future from the specified date </p>
<p>swagger/- It provides a swagger user interface for the generated API
<p>POST/{date,min temp,max temp}- It add the details of the maximum and minimum temperature for the specified date</p>
<p>For all these API the date parameter passed as input must be of the format YYYYMMDD,min/max temp is a float input</p>

<b>How to use these API</b>
<p> GET can be called using : base_url/historical</p>
<p>GET/{date} can be called using :base_url/historical/date</p>
<p>FORECAST/date can be called using:base_url/forecast/date</p>
<p>POST/{date,min temp,max temp} can be called using : base_url/{date,min temp,max temp}</p>
<p>DELETE/{date} can be called using :base_url/historical/date</p>
<p>SWAGGER can be called using :base_url/swagger</p>
