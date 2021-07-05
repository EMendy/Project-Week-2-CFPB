# Project-Week-2-CFPB
Working with complaint data from CFPD to better understand data visualization

INSTRUCTORS NOTES: 
•	At least one data-driven graphic (preferably two)
•	Some text (preferably at least three paragraphs)

Documentation of your process, which includes:
•	Link(s) to where your data came from
•	Description(s) of your data
•	Description of any cleaning, reformatting, or combining datasets
•	Description of the final analysis that you performed
END 

### Info

The CFPD was created in 2011 during the Obama Administration, driven by the work from Senator Elizabeth Warren.  The impetus for the creation of the agency was the market collapse in 2008-2009 following years of market manipulation from large financial institutions.  The Insitituion exists to support the public in their interactions with financial institutions.  In general, when a consumer feels that they have been wronged by a financial institution or had been wronged in a financial transaction with an institution, they can file a complaint with the CFPB.  It is a federally supported agency that acted, in a way, to bring to light and aggregate the complaints of seemingly small Davids against the Golaith's, much like the BBB proports to do in the private sphere.  

Being a new beaurocratic agency, the CFPB took time to ramp up and establish a "typical" amount of complaints, or, a reasonable trendline for us to analyze.  Basically, consumers didn't know the CFPB existed, and didn't know that they could file complaints, etc.  Additionally, while the Obama administration established and supported the CFPB, because the agency is part of the political complex of the executive branch, the work of the agency, and thus the effectiveness of the agenc and the public's faith in the agency to do it's job, is dependent on the administration in office and how they choose to enable/support the agency.  The Trump administration, in direct opposition to the Obama administration deliberatly acted to dismantle the CFPB.  Then and currently, the Biden administration has much in the path of the Obama administration supported the work of the CFPB once more.


### GRAPHICS
Representation of the amount of complaints filed for CFPD from initiattion to present day.  
  Marked presidential administtrations to compare differing approach to the work of the CFPB.  
  
Looking at the complaints in more detail: 
  I am going to try and recreate the map that was published on the CFPB website displaying the complaints per state.  
  
Graphic #1 Basic Visualization of the top 20 complaint garnering companies --all years--all categories

	* Exported this data into an excel: [https://docs.google.com/spreadsheets/d/1qXBvxcShVYt7H8y8d9RBGEzLpLakjvMbNU3omRo7Yuw/edit?usp=sharing ]
	* Created a graph via DataWrapper : [


### Notes - Things to consider when examping this data

Just because there are more or less complaints in a particular place, doesn’t indicate that there are more or fewer consumer financial issues.  What it might indicate is that consumers are more empowered to reach out to the CFPB to file a complaint. The CFPB is a newer organization compared to others in the federal bureaucracy, and it received particular lack of resources and support during the Trump administration’s tenure.  Government agencies do not operate or execute similarly across all administrations, and this might have led to changes in consumer behavior in interacting with the agency in the form of complaint filing. 

Complaints as compared to the population of the state 18 +
Complaints compared to political affiliation in last election
Complaints year to year over last three years
Complaints by company
Complaints by state and why?
Types of complaints

### METHODOLOGY

CFPB API is available, though the CFPB site allows you to segment the data and download just the filtered data on which you'd like to focus.  I pulled data this way into the "complaints.csv", and used pandas in a jupyter notebook to analyze the data.  

From there I segmented the data that I wanted detailing the total number of compaints per year, to understand how the complaints have changed BOTH as the CFPB has established as a beaucratic agency AND as the varied executive administrations terms overlap with its development. 

In order to do so, I created a dataset of the years and the presential administation in office during those years. 

I then combined the two data sets.  

Using DataWarapper, I created a visual of the timeline overlaid with both the complaints represented linearly, and the presidential administrations overlaid on the complaints data. 

#### Data Links: 

Link to data download : [https://files.consumerfinance.gov/ccdb/complaints.csv.zip]
Consumer Financial Protection Bureau Complaint Database
[https://www.consumerfinance.gov/data-research/consumer-complaints/search/?dataNormalization=None&dateRange=3y&date_received_max=2021-06-12&date_received_min=2018-06-12&searchField=all&state=KS&tab=Map]

[https://www.consumerfinance.gov/data-research/consumer-complaints/]


Publication Criteria for the database :
	[https://files.consumerfinance.gov/f/201303_cfpb_Final-Policy-Statement-Disclosure-of-Consumer-Complaint-Data.pdf] 

Data use documentation
	[https://www.consumerfinance.gov/complaint/data-use/]
	
API Documentation
	[https://cfpb.github.io/api/ccdb/] 
