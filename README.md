# retail-analysis-sample
This is a Doku for retail analysis sample with Power BI.

Source: 
https://docs.microsoft.com/en-us/power-bi/sample-retail-analysis from http://obvience.com/

Before going further, we need understand the concept of the data model, please read the link below:
https://en.wikipedia.org/wiki/Data_model

This analysis contains 4 entity (table) and every table has to attribute.

1. store:
* LocationID
* City Name	
* Territory	
* PostalCode	
* OpenDate	
* SellingAreaSize	
* DistrictName	
* Name	
* StoreNumberName	
* StoreNumber	
* City	
* Chain	
* DM	
* DM_Pic	
* DistrictID	
* Open Month No	
* Open Month	
* Open Year	
* Store Type

2. item
* ItemID	
* Segment	
* Category	
* Buyer	
* FamilyNane

3. time
* ReportingPeriodID	
* Period	
* FiscalYear	
* FiscalMonth	
* Month

4. district
* District	
* DM	
* DM_Pic_fl	DM_Pic	
* BusinessUnitID	
* DMImage

5. sales fact
* MonthID	
* ItemID	
* LocationID	
* Sum_GrossMarginAmount	
* Sum_Regular_Sales_Dollars	
* Sum_Markdown_Sales_Dollars	
* ScenarioID	
* ReportingPeriodID	
* Sum_Regular_Sales_Units	
* Sum_Markdown_Sales_Units


### Let's make the data model from the 4 entity. Just drag every [Primary Key](https://en.wikipedia.org/wiki/Primary_key) of the entity in power pivot or power bi data model
![retail analysis sample data model](https://user-images.githubusercontent.com/27078712/40864635-e6a6188e-65f4-11e8-8d18-22021f05a6d5.PNG)

### After that, create [a measure in power bi or power pivot](https://docs.microsoft.com/en-us/power-bi/desktop-tutorial-create-measures)

Below are the measure of every graph,

Note! we use the format of table and attribut with [DAX language](https://docs.microsoft.com/en-us/power-bi/desktop-quickstart-learn-dax-basics) 

Extras: [Quick Guide DAX](https://support.office.com/en-us/article/quickstart-learn-dax-basics-in-30-minutes-51744643-c2a5-436a-bdf6-c895762bec1a?omkt=en-US&ui=en-US&rs=en-US&ad=US)

---------------------------------------------------------------------------
Drag this entity for every graph

* This Year Sales by Chance graph:



1. (Store)[Chain] 

2. (Sales)[This Year Sales] := [TotalSalesTY]

DAX -> TotalSalesTY = CALCULATE([TotalSales], Sales[ScenarioID]=1)

* New Stores graph: 
.
.
.coming soon




