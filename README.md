# Sample Holiday Schedules & Holidays
## Introduction
Admins canmay now define holidays directly in Vault using the Holiday Schedule and the Holiday objects. You can think of Holiday Schedule records as countries or regions and Holiday records as the individual dates for the holidays within a certain country. For example, you might define one Holiday Schedule record as Uniteds States, and then create children Holiday records for each holiday for all the relevant years., In this scenarioeg, you would create a separate record for each year you would like to count President's Day as a holiday.
Holiday Schedule records can may then be associated with user records, and may be used in expressions through Vault with the NetWorkdays() and Workday() functions. These functions allow you to calculate the difference between two dates factoring out weekends and holidays, and return a date that is N business days in the future. 

## Description of VPK
To help Aadmins get started, we have created this VPK containing sample Holiday Schedule and Holiday records. Included in the package are 63 countries and their associated holidays from 1950 through 2049. Below, you can see a list of all of the countries and regions included. This package was created using the publicly available [holidays](https://pypi.org/project/holidays/) project version 0.12.

**Included countries and regions:**
Argentina, Australia, Austria, Bangladesh, Belgium, Brazil, Bulgaria, Canada, Chile, Colombia, Croatia, Denmark, Egypt, England, Estonia, Finland, France, Georgia, Germany, Greece, Hong Kong, Hungary, Iceland, India, Ireland, Israel, Italy, Japan, Korea, Latvia, Lithuania, Luxembourg, Malaysia, Mexico, Morocco, Netherlands, New Zealand, Nicaragua, Nigeria, Northern Ireland, Norway, Peru, Poland, Portugal, Romania, Russia, Saudi Arabia, Scotland, Serbia, Singapore, Slovakia, Slovenia, South Africa, Spain, Sweden, Switzerland, Turkey, Ukraine, United Arab Emirates, United Kingdom, United States, Vietnam, Wales
## How to deploy the VPK
To use this VPK as sample data in your Vault:
1. Download the `all_holidays.vpk` file.
2. Navigate to **Admin > Deployment > Inbound Packages**, click **Import** and select `all_holidays.vpk`. You will receive a notification when Vault finishes importing the package.
3. From the Actions menu next to the package name, select Review & Deploy.
4. Click Next, then click Finish.

If successful, this package will create 63 Holiday Schedule records and 88,153 Holiday records. To avoid confusion, we recommend confirming there areis no existing Holiday Schedule records in your Vault that overlap with those being uploaded.
## License
This VPK serves as an example and is not meant for production use. Veeva does not guarantee the accuracy of the data included in this package.

