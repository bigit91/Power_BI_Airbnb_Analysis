# Power_BI_Airbnb_Analysis
Here I have analyzed an Airbnb dataset and made a short and detailed analysis report on the property listings across a specific area and its neighborhood
# AIRBNB Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/b2ec7de1-b0af-4532-886b-60d75d27aa0e/ReportSection?experience=power-bi

### Introduction :

Since 2008, guests and hosts have used Airbnb to expand on traveling possibilities and present more unique, personalized way of experiencing the world. 
This dataset describes the listing activity and metrics in NYC, NY for 2019.
Airbnb, Inc. is San Francisco, California based company which act as a broker and provides an online marketplace for short-term homestays. 
The company charges a commission from each bookings. Aibnb providing it premium service and experience to customers  since 2008. Today Airbnb has millions of listings.
These listings generates lost of data. Analyzing this data become crucial factor for the company. This data can be use for business decisions, marketing, implementations of initiatives, additional services and much more.


### Problem Statement:	Given dataset include all information about host, listed properties, geographical location, prices reviews and all other required metrics. 
		      	Analyse the given dataset make different predictions and draw meaningful conclusion in order to grow the business. 
		      	Also state what can we learn from different predictions.  
		      	Inspiration:
  		        ● 	What can we learn about different hosts and areas?
			        ●  	What can we learn from predictions? (ex: locations, prices, reviews, etc)
			        ●  	Which hosts are the busiest and why?
			        ●	  Is there any noticeable difference of traffic among different areas and what could be the reason for it?

### About Dataset :	This dataset has round  48895 listings and  16 Columns. It is mix between categorical and numeric values. 
		  	Given dataset contains null values as blanks  well which we have to consider while doing analysis. Last_review and reviews_per_month has more null values. 
			There are 5 neighbourhood group in which all listings located. Nearly 80-85% of listings located in Manhattan and Brooklyn. 
			In Manhattan booking price is bit higher as compared to other neighbourhood groups. There are 3 kind of room type (i.e Shared Room, Private Room, Entire home/Apt).
			Out of which Shared room are least preferred by the customer even after having less price for booking. 


### Columns Present in dataset are : Id : Listing ID of the property
					Name : Name of the listed property.
					host_id : ID of the property owner.
					host_name : Name of the property owner.
					neighbourhood_group : Location at which property located.
					Neighbourhood : Area in which property located.
					Latitude : Latitude coordinate. 
					Longitude : Longitude coordinate.
					room_type : Type of the room (Entire Home/ Appt, Private Room, Shared Room)
					Price : Price in Dollars.
					Minimum_nights : Amounts of minimum night stay at property
					number_of_reviews : No. Of reviews
					last_review : last review on which date.
					reviews_per_month : Numbers of reviews per months.
					calculated_host_listings_count : Count of properties listed on that host.
					availability_365 : Number of days when listing is available for booking


### Questions :
		1.	In which Neighbourhood group there is maximum number of properties listed ?
		2.	Which host has maximum number of properties listed ?
		3.	What is the average price in different properties listed ?
		4.	What may be the reason of having high price in that neighbourhood groups ?
		5.	What is the most prefered room type in the every neighbourhood groups ?
		6.	Total availability of properties having different room type?
		7.	Which one is the busiest host ?
		8.	Which property has maximum number of reviews ?

### Analysis Questions 👍

		* Show total room types

		* Find the total number of shared rooms, private rooms, entire  home/apt

		* Create a slicer for dates to show last reviewed information

		* The prices for each neighborhood group

		* Create a table for host to check the count of properties been listed for each neighborhood group.






### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : It was observed that  there were some null values in few columns which were replaced by zeroes 0 as suggested by stakeholder
- Step 4 : In the report view, under the view tab, theme was selected . along with it Canvas background was selected in the Format Section of the Visualizations Pane
- Step 5 : We Start with the  Overview
			1) Title of the page was created using textBox and name it as Airbnb Data analysis
			2) 4 Cards were created  to show the "Max Reviewed property","Neighbourhood where Max property was listed","Host With Max properties Listed" , "And Average property Price"
			3) Next a table  was created to show  "Host wise property Listings" which was arranged in the descending valuess of the Host wise total property listings 
			4) Another table was created to show " Neighbourhood wise total Host  property listings" arranged the descending values of the Host wise total property listings 
  			5) In another table Room type and "Availibility Count"  was shown
			6) Also Room wise total reviews was shown in a table to analyze which was the most booked room
			7) Lastly we create month wise count of Reviews 
- Step 6: We Create an Analysis page 
			1)We Create 3 Cards to Show the different categories of the room viz , "Entire home/apt", "Private room" ," Shared  Room"
			2) A donut Chart is created to show the Type of Rooms by its Count along with the overall percentage 
			3) A stacked  horizontal bar chart is created to analyze "max reviewd property" sorted by the descending values of the review 
			4) A Funnel Chart is created  to visualize the  "Avg Proprty price by Neigborhood Group "
			5) then we create a matrix to visualize  the Number of Property by Top 5 host in each Neighbourhood Group
			6) We place a date slicer in order to filter the fields by date 

 
Insights :
		1) Neighbourhood group where max properties are listed is  "Manhattan"  

![Air3(Neighborurhood)](https://github.com/bigit91/port1/assets/155818756/bf2d1f08-69f1-4d21-88b4-13535a6cbfde)


		2) Host with max properties listed is "Michael" 

![Host With max prop](https://github.com/bigit91/port1/assets/155818756/5b6d5ca8-a52f-4535-8950-72d5a1a81069)

		3) Average Price of the different Properties  listed  is  " $160.21 "
![Air1](https://github.com/bigit91/port1/assets/155818756/e412988b-189b-422f-b8f2-b4bc6994fbd1)


		
		4) The  reason for high price in Manhattan is beacause of  Max number of properties are listed in that particular neighbourhood which means it ha highet footfall of guests

		
		5) The most preffered room type in every neigbourhood group is "Entire Home /Apt "

		
		6) Total Availability of  properties having different room types are  
			a) Entire Home/Apt   - 366
			b) Private Room      - 366
			c) Shared Room 	     - 232

		7) Michael is the busiest host with total 416 Listings 

		
		8) "Room Near Jfk Queen Bed" was the Max reviewed property
		
![Air2](https://github.com/bigit91/port1/assets/155818756/1b1ed57f-4f11-41ec-82d5-ca96a4e46b15)

		
		9) Reviews per month :
					Jan - 218
					Feb - 170
					March -203
					Apr -263
					May -405
					June -801
					July -830
					Aug -133
					Sept -139
					Oct -151
					Nov -155
					Dec -199
				We observe that  peak reveiws were recorded in the month  of June and July 

![Reviews Per Month](https://github.com/bigit91/port1/assets/155818756/9dc1beb2-d732-48ff-b06c-438c615de21a)


		10) Average Price foe eaach neigbourhood Group :  
				Manhattan : $175.67
				Brooklyn   : $120.29
				Queens	  : $98.29
				Staten Island : $94.29
				Bronx : $78.78
		
	
Dashboard Snaps :
	
![Overview](https://github.com/bigit91/port1/assets/155818756/ec50d993-503e-49ee-bedd-36e3eae00640)

![Analysis](https://github.com/bigit91/port1/assets/155818756/f1dd87b6-230f-4358-a2c7-3404783d24d4)

	




		
