In today’s business world, Environmental, Social, and Governance (ESG) factors are more critical than ever. While environmental and governance issues often get the most attention, the social aspect—which includes the human elements related to society, communities, and individuals—is equally important. Tracking and analyzing social metrics provides valuable insights into areas such as employee engagement, human rights, health and safety, training programs, gender pay gaps, and diversity, equity, and inclusion.

IBM Envizi helps organizations capture these essential social and governance metrics. With Envizi, companies can collect data on important social aspects, such as employee onboarding and offboarding, and issues related to modern slavery. This data can be transformed into detailed and actionable Power BI reports, enabling organizations to make better decisions and foster a more socially responsible and inclusive workplace.

In this tutorial, we will explore how organizations can capture social metrics related to employee onboarding and offboarding, as well as aspects related to modern slavery, and create comprehensive Power BI reports from this data.

To get more information about IBM Envizi or to try it out yourself, start your [14-day IBM Envizi ESG Suite trial](https://www.ibm.com/account/reg/us-en/signup?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-504&formid=urx-51938&cm_sp=ibmdev-_-developer-_-trial). You can also request a personalized [IBM Envizi demo](https://www.ibm.com/account/reg/us-en/signup?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-504&formid=DEMO-envizi&cm_sp=ibmdev-_-developer-_-trial).

## Prerequisites

- Ensure you have access to an Envizi instance with the `Account Style Wizard` enabled.
- Confirm that you have the `PowerReport Edit` work role added.

## Steps

### Step 1. Enable social metrics

To display social metrics-related data in the monthly dataset of the Power BI report, you need to enable social metrics in the Organization Settings. Request the Product team to enable social metrics in the `Organization Settings` of the Power BI report.

![image1.png](./images/image1.png)

### Step 2. Create account styles

Create account styles for the social metrics-related data. Let's create two account styles with the following information.

- **Account Style 1: Emp Hires**

	This account style helps to maintain the Employee Engagement details of the organization. It contains information such as gender, total employee count, age-wise count, and the number of employees joined, relieved, and dismissed.

  1. Go to `Admin` > `Account Style Wizard`.

     ![image20.png](./images/image20.png)

  2. Create an account style with the following settings:

		- Scope: Social Metrics
		- Data Type: People - Headcount [Number]
		- Primary Column: Qty
		- Secondary Columns: Gender, Age-21-30, Age-31-40, Age-41-50, Joining, Leaving, dismissed (Fired)

	 ![image21.png](./images/image21.png)

     ![image22.png](./images/image22.png)

- **Account Style 2: Modern Slavery**

	This account style helps to maintain the modern slavery details of the organization. It contains information such as forced labour, child labour, others, and country details.

   1. Create an account style with the following settings:

		- Scope: Social Metrics
		- Data Type: People - Headcount [Number]
		- Primary Column: Forced Labour
		- Secondary Columns: Forced Labour, Child Labour, Others, Country

   2. You can create the required fields in the account style as shown in the following figure.

   	  ![image23.png](./images/image23.png)

- **Account Style 3: Forest Conservation**

	This account style helps to maintain the forest conservation details of the organization. It contains information such as converstation type, conservation area name and area details.

   1. Create an account style with the following settings:

		- Scope: Social Metrics
		- Data Type: Social Metrics
		- Primary Column: Area
		- Secondary Columns: Conservation Type, Area Name, UnitOfMeasure

   2. You can create the required fields in the account style as shown in the following figure.

   	  ![image24.png](./images/image24.png)


### Step 3. Create accounts

Create accounts using the account styles created above, as shown in the following figures:

![image30.png](./images/image30.png)

![image31.png](./images/image31.png)

![image32.png](./images/image32.png)


Follow these steps:

1. Download the following sample files:

	- [Envizi_SetupConfig_SG_Report.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/nYync-XLp7iSxTORMYctew/Envizi-SetupConfig-SG-Report.xlsx  "Envizi_SetupConfig_SG_Report.xlsx") 
	- [Account_Setup_and_Data_Load-G5-Hires.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/YwuvwsVjxicrCCt_bBP7Tg/Account-Setup-and-Data-Load-G5-Hires.xlsx "Account_Setup_and_Data_Load-G5-Hires.xlsx").
	- [Account_Setup_and_Data_Load_G5-Slavery.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/BTgSq_Vg5aETQoSOMJxJZQ/Account-Setup-and-Data-Load-G5-Slavery.xlsx "Account_Setup_and_Data_Load_G5-Slavery.xlsx").
	- [Account_Setup_and_Data_Load-G5-Forest.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/BTgSq_Vg5aETQoSOMJxJZQ/Account_Setup_and_Data_Load-G5-Forest.xlsx "Account_Setup_and_Data_Load-G5-Forest.xlsx").

2. Make the required changes such as updating `Organization`, `Organization Link` and `Account Style Link` columns.

3. Upload the files. Go to `Manage` > `Data Files` > `Upload Files screen`.

	![image32.png](./images/image33.png)

### Step 4. Create Power BI report

After the account styles are created, wait for a day for the daily refresh to occur. This allows the newly created account styles to be reflected in the Monthly Data Set of the Power BI report.

The account styles we created will be visible in PowerReport after a day. For more information about creating custom PowerReports in Envizi, see [Creating custom PowerReports in Envizi](https://developer.com/tutorials/awb-create-custom-power-reports-in-envizi/).

![image40.png](./images/image40.png)

View the Social Metrics PowerReport as shown below.

![image41.png](./images/image41.png)

![image42.png](./images/image42.png)

![image43.png](./images/image43.png)

## Useful resources

- [PowerBI Training](https://yourlearning.ibm.com/activity/PLAN-8FF21DDE262D?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-Creating+Custom+Envizi+PowerBI+Report+for+Social+Metrics_v1_1718260961)

- [Design effective reports in Power BI](https://learn.microsoft.com/en-us/collections/o4dhk4z8xpr8q)

- [Monthly Dataset - Glossary - Basic Fields](https://knowledgebase.envizi.com/home/monthly-dataset-glossary)

- [Monthly Dataset - Glossary - Advanced Fields](https://knowledgebase.envizi.com/home/monthly-dataset-glossary-advanced-fields)

- [Monthly Dataset - Tutorials](https://knowledgebase.envizi.com/home/monthly-dataset-tutorials)

## Summary and next steps

In conclusion, IBM Envizi ESG Suite provides a comprehensive solution for creating custom PowerReports with the social and governance data of your organization.

To get more information about IBM Envizi or to try it out yourself, start your [14-day IBM Envizi ESG Suite trial](https://www.ibm.com/account/reg/us-en/signup?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-504&formid=urx-51938&cm_sp=ibmdev-_-developer-_-trial). You can also request a personalized [IBM Envizi demo](https://www.ibm.com/account/reg/us-en/signup?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-504&formid=DEMO-envizi&cm_sp=ibmdev-_-developer-_-trial).