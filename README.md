<h1 align="center">Final Report<br>Assignment By: Derek Evans<br>Submitted On: Jan. 20th, 2019</h1>

<p>The main scope of this project is to deploy an automated data collection solution using the <a href="https://www.ibm.com/watson/index.html" target="_blank">Watson Studio</a> data science platform in conjunction with a <a href="https://www.ibm.com/cloud/db2-on-cloud" target="_blank">IBM DB2 on Cloud</a> database.  In developing this solution, my intention was to solve a problem that was mentioned by one of the instructors from the Data Science Methodology course of this program.  During one of the course presentations, the instructor had placed an emphasis on mentioning that one of the most difficult and time-consuming aspects of the data science process is data collection, processing, and generation of new data.  While I'm not a data scientist by any means, I can relate to and agree that the amount of worked involved in preparing data for any kind of analysis and, or research is not only difficult, but exhausting.  This is the type of work that often has little to no reportable production output and depending on the circumstances, can come under a great deal of criticism as the allocation of human capital towards such efforts are costly. </p> 

<p>By using a series of multiple of <a href="https://jupyter.org/" target="_blank">Jupyter</a> notebooks and a cloud database, I was able to not only automate the data collection process in retrieving data from the Foursquare API database, but also generate new data as well.  When a user performs a location-based trending search using any of the <a href="https://foursquare.com/" target="_blank">Foursquare</a> applications or API calls, the search results will only return trending data based on the number of users currently checked in at a location at the time the search is executed.  Once the browser or application is closed, the user no longer has access to the information provided in that search.  Which is one of the issues this project solves, by simply executing an API call that performs a trending search and stores the search results in a database for permanent storage.  In doing this, the database will have historical time-series trending venue data capable of producing useable data in real-time with preestablished time delay. </p>

<p>Now, I'm sure Four squares already have this data and offers it to customers through one of its premium subscription services, which starts off at around $600 a month, but I couldn’t find solid historical data of this nature through any other channels offered with the unpaid developer’s subscriptions.  The closest thing I found was the <a href="https://developer.foursquare.com/docs/api/venues/details" target="_blank"><strong><em>Popular</em></strong></a> response field under the <a href="https://developer.foursquare.com/docs/api/venues/details" target="_blank"><strong><em>Get Venue Details</em></strong></a> endpoint API call.  This endpoint will give users a range of operating hours when the specific location searched has the most amount of traffic.  This information doesn't give me a weighted value of any nature to compare how popular the venue is at that time in relationship to other venues. </p>

<p>I'll be fourth coming in pointing out that intent of this project was to develop a solution which aims to accurate the data collection and processing stages of the data science methodology.  Most of my time was focused on developing a solution to improve aid in future data science projects to come.  I was able to generate new time series data using the trending venue API call.  This data can be viewed in the <a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Analysis%20and%20Report.ipynb" target="_blank">Analysis and Report</a> notebook stored in my GitHub repository, which is one of the 15 notebooks utilized for this project.  The following list provided below contains links to the notebooks that we're utilized throughout the course of the project, not including the numerous testing files generated throughout the troubleshooting process. </p>

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

<h3 align="center"><a href="https://share.mindmanager.com/#publish/5Q7GMjJ-1gXEDz4VOR68-SEZmFcPAlOZZmjFhl2R" target="_blank">Project Diagram</a></h3>

<hr>

<img src="https://fgy7oa.dm.files.1drv.com/y4mOktvWwvwzHpJl87YCdPKjhoA2hEen9Jv71BP-u4Lgn59TxcB6JvEaY7z4W90SEq5TPeza21zVu-JlOWn_KXn7szHSOZMSVvN45jZ3ITV6daRgtMOSuisIrQEcPIxTzwt57kzXfmNrVSvI8mmcNorkzY6LOSocYQBryPJAMtyES1Ut6r8ip9jN6tW8I2OmQkxY1jKYVZYvhJfBSn0FT27ow?width=1388&height=803&cropmode=none" width="1024" height="592" />

<hr>

<p>The Data Retrieval notebook was created as a work around and will eventually be eliminated, unless another purpose for it is found.  This was added to the scope of the project as a temporary solution for exceeding my maximum daily API call limits which is capped at 950 calls per day.  One of the problems I've been having throughout the course of the project, is inconsistent data being returned when performing an API call to the Foursquare database.  Based on my observations, the search results vary based on the city and venue identified in the search.  While I'm not completely sure, I believe venue plays a more significant role in the variations, however the differences tend to be somewhat consistent from one city to the next.  In addition to this, I've noticed that since I've began working on this project, the incoming data has been changing leading me to be believe that the records contained in the database are being updated simultaneously.  The reason this becomes an issue, is I've been working to program exceptions into the data collectors in order to produce consistent data frame priors to submitting the data frame to the DataSciDB database. </p>

<p>If you review the results generated by the data collectors in the <strong><a href="https://github.com/REPNOT/Coursera_Capstone/blob/master/Final%20Assignment%20-%20Analysis%20and%20Report.ipynb" target="_blank"><em>Analysis &amp; Report Notebook</em></a></strong> you'll notice that the data isn't uniform in the dataframe.  In order to produce an auto generated data sample for this project, I had to let start letting some of the unprocessed data through to the final dataframe in order to get results sent to the DataSciDB database for storage.  From there the data is retreived and processed in the Data Retrieval notebook.</p>

<p>The most critical aspect of the project is the data collectors, which handle all of the hard work by performing API calls, retreiving the search results, processing the incoming data, and sending it to the database for retreival.  Originally, I only intended to use four data collectors that would be scheduled to run every hour 15 minutes apart.  As a means of producing a large enough data set for finishing this project, I increased that number to 12 and scheduled each one to run hourly, five minutes apart from one another.  This resulted in a lot of overlapping data that probably isn't necessary, but it does provide a good example of the system capabilities available with the IBM Watson Studio platform.  Once I started letting unprocessed data through, the program worked excellent.  I monitored the Trending Data table in the DataSciDB during the process and the database was automaically refreshing as new data came in.</p>

<p>Going forward, if I can continue to add exceptions to accommodate the search result variations, the Analysis &amp; Reporting can be scheduled to run hourly, so every time a user we're to access the notebook, they would be looking at updated data results and visualizations without having to rerun the program.  This program still needs a lot of work, with a focus on creating a secondary database table to act as a cache for results falling outside of current exception parameters.  This will be helpful in planning future adjustments and prevent program errors that are likely to occur when data is sent to the database. </p>

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

<h2>Final Assignment</h2>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/4ccf352d-d267-409c-8651-bd34d060e341/view?access_token=b546245032c3671b505611d1ac408893fe52cdf2c7123a1476dd26e7d1e19912" target="_blank">Final Report</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/ed945533-ff35-4d1d-a02e-4af956f1986a/view?access_token=9e6ed08d23aea24139e923a336730ea516c1645ca8b2a23faf0c87d4bd4c8981" target="_blank">Analysis & Report</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/d898d40d-2f00-404a-81ff-d939e756d16a/view?access_token=f349d8b27951ddc429668f1b2f9f05a73c423f7753481872d781ce33c0bf6579" target="_blank">Data Retrieval</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/7eff4c08-6060-4285-8e8b-3d2c4b956e92/view?access_token=99498c3045c221c12b0d578b86186e476e384385d18d9a35cdd1293658b33d3e" target="_blank">Web Scraper</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/dc3e838d-0440-4031-9791-99c49015828f/view?access_token=ccd77c0bf2ee61703cd319244c0de44171ed9c1ba9e7d4a55a68c2c2c2f51e89" target="_blank">Data Collector 1</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/92c07694-4845-46c9-9391-40c1c49e2f16/view?access_token=490a725d635dd394201e4e3112b185960f4ec421c9d8aa1a7c72a21b221bbddf" target="_blank">Data Collector 2</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/92c07694-4845-46c9-9391-40c1c49e2f16/view?access_token=490a725d635dd394201e4e3112b185960f4ec421c9d8aa1a7c72a21b221bbddf" target="_blank">Data Collector 3</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/ba6af1e1-654c-4640-86b5-8cf8ea8a22ca/view?access_token=c8c8826fce399fb220b11a034add1eddae25cad70d967dd9be8c756feb353920" target="_blank">Data Collector 4</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/57eeccec-7465-4595-b7a5-90da66e944af/view?access_token=b4448813af561a59aaeb642035881fefd33c41f601d548d7ab6b929139a9a8ab" target="_blank">Data Collector 5</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/9efa4a48-abfe-4530-bd25-bd5f354bc9eb/view?access_token=c776db7b210d89f90f32682f3562c7c0339bc850a6492b67f049027de28ff829" target="_blank">Data Collector 6</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/2b9d054c-51ff-4d73-8a6c-e7f449a635c5/view?access_token=2daa3402da257e39d5a3a634e4a8f0675594a235201b57d1f3f9c0b893a7528b" target="_blank">Data Collector 7</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/15eff95b-0bc7-4731-a09a-a54e81dcb4b9/view?access_token=495bbaee6c83b5998afd6e2c648e95e48b9451446549b32f6263dc1614b8cde7" target="_blank">Data Collector 8</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/98f7e119-5859-4469-b48b-3019d561cc7c/view?access_token=f154cab6e7b76fdafe65cda279e30055ba70cdccbafb7f6575a82cf6ffde32b4" target="_blank">Data Collector 9</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/8ac500b0-f82d-4534-8060-b1180930e408/view?access_token=80e77c0b0500acb97259ac42071cefd52f77d272cb7aafbca8b698738983f119" target="_blank">Data Collector 10</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/1c778a50-25ed-4512-adfb-f8a58951cfd6/view?access_token=f2d8a23b6478d34d0f9143a18fce6abfe1f46777041adc8fc6997ffb9b008b8b" target="_blank">Data Collector 11</a>

<a href="https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/4e7f13be-2cb0-4b13-ad6e-ac3bd32c7c2f/view?access_token=61a7faae9465e77294937923faf4579feaa8e6d161f10daa9efedb488e4f9a64" target="_blank">Data Collector 12</a>

<hr>
