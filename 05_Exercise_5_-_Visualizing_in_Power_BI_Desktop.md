# Exercise 5: Visualizing in Power BI Desktop

Duration: 20 mins

Synopsis: In this exercise, attendees will construct a report in Power BI Desktop Client that uses the map visualization to illustrate the predicted delays, using the data originally scored using Machine Learning, and stored in SQL Azure.

This exercise has 4 tasks:

* [Task 1: Connect to the Azure SQL Database Using Power BI Desktop](#task-1-connect-to-the-azure-sql-dataabse-using-power-bi-desktop)
* [Task 3: Create Power BI Report](#task-3-create-power-bi-report)

## Task 1: Connect to the Azure SQL Database Using Power BI Desktop

1. Launch Power BI Desktop.
2. Click on **Get Data** from the left side of the welcome window.

    ![Screenshot](images/connect_to_the_hdinsight_spark_using_power_bi_desktop_0.png)

1. Click on the **Azure** from the left and select **Azure SQL Database** from the new **Get Data** window. Click on the **Connect** button on the bottom right corner.

    ![Screenshot](images/ex06_power_bi_1.png)

1. Enter the name of the server and database on the **SQL Server Database** screen.

    ![Screenshot](images/ex06_power_bi_2.png)

1. Switch the authentication mode to **Database**, and enter the username and password.
2. Click **Continue** on the bottom right corner of the new window.

    ![Screenshot](images/ex06_power_bi_3.png)

1. Click the **ScoredFlightData** table, and click **Load**.

    ![Screenshot](images/ex06_power_bi_4.png)

## Task 2: Create Power BI Report

1. Once the data load is completed, you will find the **ScoredFlightData** to the right side of the screen under the **Fields** area.

    ![Screenshot](images/create_power_bi_report_0.png)

1. From the **Visualizations** area, which is left to the **Fields** area, click the **Globe** icon to add a Map visualization to the report design surface.

    ![Screenshot](images/create_power_bi_report_1.png)

1. With the Map visualization still selected, in the **Fields** area at right, expand the tabled called **flightdelayssummary**.

    ![Screenshot](images/create_power_bi_report_2.png)

1. Click and drag the field labeled **OriginLatLong** and drop it into the **Location** field located just below visualizations.

    ![Screenshot](images/create_power_bi_report_3.png)

1. Next, drag the field labeled **NumDelays** and drop it into the **Size** field.

    ![Screenshot](images/create_power_bi_report_4.png)

1. Your map should look something like the following:

    ![Screenshot](images/create_power_bi_report_5.png)

1. Unselect the Map visual by clicking on the white space on the report page.
2. From the **Visualizations** area, which is left to the **Fields** area, click the **Stacked Column Chart** icon to add a bar chart visualization to the report design surface.

    ![Screenshot](images/create_power_bi_report_6.png)

1. With the **Stacked Column Chart** visualization still selected, in the Fields area at right, expand the tabled called **flightdelayssummary**.

    ![Screenshot](images/create_power_bi_report_7.png)

1. Click and drag the field labeled **Day** and drop it into the **Axis** field located just below visualizations.

    ![Screenshot](images/create_power_bi_report_8.png)

1. Next, drag the field labeled **AvgDelayProbability** and drop it into the **Value** field.

    ![Screenshot](images/create_power_bi_report_9.png)

1. Grab the corner of the new **Stacked Column Chart** Visual and drag it out by making wide as the bottom of your report design surface.
2. Your report should look something like the following:

    ![Screenshot](images/create_power_bi_report_10.png)

1. Unselect the Stacked Column Chart visual by clicking on the white space on the report page.
2. From the **Visualizations** area, which is left to the **Fields** area, click the **Treemap** icon to add this visualization to the report design surface.

    ![Screenshot](images/create_power_bi_report_11.png)

1. With the **Treemap** visualization still selected, in the Fields area at right, expand the tabled called **flightdelayssummary**.

    ![Screenshot](images/create_power_bi_report_12.png)

1. Click and drag the field labeled **OriginAirportCode** and drop it into the **Group** field located just below visualizations.

    ![Screenshot](images/create_power_bi_report_13.png)

1. Next, drag the field labeled **NumDelays** and drop it into the **Value** field.

    ![Screenshot](images/create_power_bi_report_14.png)

1. Grab the corner of the new **Treemap** Visual and drag it out by making wide as the top of your report design surface. Your report should look similar to the following:

    ![Screenshot](images/create_power_bi_report_15.png)

1. You can cross filter the visualizations on the report by click on the one of the other visuals within the report as shown below.

    ![Screenshot](images/create_power_bi_report_16.png)

1. You can save this Power BI report by click on Save icon from the top left corner of the screen.

Next Exercise: [Exercise 7 - Deploy Intelligent Web App](07_Exercise_7_-_Deploy_Intelligent_Web_App.md)
