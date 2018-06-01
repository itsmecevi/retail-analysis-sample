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


### Let's make the data model from the 4 entity. Just drag every Primary Key of the entity in power pivot or power bi data model
![retail analysis sample data model](https://user-images.githubusercontent.com/27078712/40864635-e6a6188e-65f4-11e8-8d18-22021f05a6d5.PNG)




