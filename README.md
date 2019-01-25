<h1 align="center">Data Science Capstone: Final Assignment Submission</h1>

<h2 align="center">Final Report</h2>
<h2 align="center">Assignment By: Derek Evans</h2>
<h2 align="center">Submitted On: Jan. 20th, 2019</h2>

<p>The main scope of this project is to deploy an automated data collection solution using the <a href="https://www.ibm.com/watson/index.html" target="_blank">Watson Studio</a> data science platform in conjunction with a <a href="https://www.ibm.com/cloud/db2-on-cloud" target="_blank">IBM DB2 on Cloud</a> database.  In developing this solution, my intention was to solve a problem that was mentioned by one of the instructors from the Data Science Methodology course of this program.  During one of the course presentations, the instructor had placed an emphasis on mentioning that one of the most difficult and time-consuming aspects of the data science process is data collection, processing, and generation of new data.  While I'm not a data scientist by any means, I can relate to and agree that the amount of worked involved in preparing data for any kind of analysis and, or research is not only difficult, but exhausting.  This is the type of work that often has little to no reportable production output and depending on the circumstances, can come under a great deal of criticism as the allocation of human capital towards such efforts are costly. </p> 

<p>By using a series of multiple of <a href="https://jupyter.org/" target="_blank">Jupyter</a> notebooks and a cloud database, I was able to not only automate the data collection process in retrieving data from the Foursquare API database, but also generate new data as well.  When a user performs a location-based trending search using any of the <a href="https://foursquare.com/" target="_blank">Foursquare</a> applications or API calls, the search results will only return trending data based on the number of users currently checked in at a location at the time the search is executed.  Once the browser or application is closed, the user no longer has access to the information provided in that search.  Which is one of the issues this project solves, by simply executing an API call that performs a trending search and stores the search results in a database for permanent storage.  In doing this, the database will have historical time-series trending venue data capable of producing useable data in real-time with preestablished time delay. </p>

<p>Now, I'm sure Four squares already have this data and offers it to customers through one of its premium subscription services, which starts off at around $600 a month, but I couldn’t find solid historical data of this nature through any other channels offered with the unpaid developer’s subscriptions.  The closest thing I found was the <a href="https://developer.foursquare.com/docs/api/venues/details" target="_blank"><strong><em>Popular</em></strong></a> response field under the <a href="https://developer.foursquare.com/docs/api/venues/details" target="_blank"><strong><em>Get Venue Details</em></strong></a> endpoint API call.  This endpoint will give users a range of operating hours when the specific location searched has the most amount of traffic.  This information doesn't give me a weighted value of any nature to compare how popular the venue is at that time in relationship to other venues. </p>

<p>I'll be fourth coming in pointing out that intent of this project was to develop a solution which aims to accurate the data collection and processing stages of the data science methodology.  Most of my time was focused on developing a solution to improve aid in future data science projects to come.  I was able to generate new time series data using the trending venue API call.  This data can be viewed in the <a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Analysis%20and%20Report.ipynb" target="_blank">Analysis and Report</a> notebook stored in my GitHub repository, which is one of the 15 notebooks utilized for this project.  The following list provided below contains links to the notebooks that we're utilized throughout the course of the project, not including the numerous testing file generated throughout the troubleshooting process. </p>

<ul>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Web%20Scraper%20%20.ipynb" target="_blank">Web Scraper Notebook</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Retrieval.ipynb" target="_blank">Data Retrieval Notebook</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Analysis%20and%20Report.ipynb" target="_blank">Analysis &amp; Report Notebook</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%201.ipynb" target="_blank">Data Collector 1</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%202.ipynb" target="_blank">Data Collector 2</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%203.ipynb" target="_blank">Data Collector 3</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%204.ipynb" target="_blank">Data Collector 4</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%205.ipynb" target="_blank">Data Collector 5</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%206.ipynb" target="_blank">Data Collector 6</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%207.ipynb" target="_blank">Data Collector 7</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%208.ipynb" target="_blank">Data Collector 8</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%209.ipynb" target="_blank">Data Collector 9</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%2010.ipynb" target="_blank">Data Collector 10</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%2011.ipynb" target="_blank">Data Collector 11</a></strong></li>
    <li><strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Data%20Collector%2012.ipynb" target="_blank">Data Collector 12</a></strong></li>
</ul>


<p>The data contained in the Analysis and Report notebook is a combination of data generated by the Web Scraper notebook that was used in the Data Collectors, along with new data produced by the data collectors.  For the actual data that was used or, can be used to perform an analysis, I was able to collect trending venue data for various cities in five-minute intervals spanning a period of 5 hours and 36 minutes on Sunday, Jan. 20th, 2019.  While this is not a significant amount of data, it was generated autonomously using the following structure shown in the diagram below. </p>

<h1>Coursera Capstone<br>IBM Applied Data Science on Coursera</h1>

<p><strong>Capstone project repository for the IBM Data Science program offered on Coursera.</strong></p>

<hr>

<h2>Week 1</h2>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/7db28247-dda8-4f3c-83ab-70cb7f490ee3/view?access_token=bf1ae629e104b08c8628498e05f3262803a41144b138400f2d6a9a10490d875f" target="_blank"><strong>Week 1 Assignment Submission<strong></a>

<hr>

<h2>Week 3</h2>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/12f6a03d-d8bd-4512-aad8-cbeb896163aa/view?access_token=241ba308286f238ea299fe3f9fb5945561db457000c29927114785e3029a6e85" target="_blank"><strong>Week 3 Assignment Submission - Part 1<strong></a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/55e82a97-face-4273-b38c-f30ca795bd4f/view?access_token=fbe71a70048347ccbf7473ebc1d7c4303d74f4a2904ca3cfa8853cc0b11a99f0" target="_blank"><strong>Week 3 Assignment Submission - Part 2<strong></a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/de556fbc-fdb1-4c39-8be9-4494c0862ed2/view?access_token=236d55a02e8a2cac3f50f24cbf3fbddcb6c844041bbaf5078dc5190f9942fa09" target="_blank"><strong>Week 3 Assignment Submission - Part 3<strong></a>

<hr>
