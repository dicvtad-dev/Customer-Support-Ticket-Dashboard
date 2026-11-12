# Customer Support Ticket Analytics Dashboard \| Power BI

An interactive Power BI project for exploring customer support ticket
volume, ticket status, issue categories, priority levels, support
channels, team assignments, city distribution, response times,
resolution times, and agent-level activity.

**Created by:** Divyesh Tadvi\
**Tool:** Microsoft Power BI Desktop

## Project overview

This project uses a customer support ticket dataset containing **400
ticket records** and **16 fields**. The report presents operational
views of ticket handling and customer support activity, with filters for
dimensions such as city, priority, channel, status, issue category,
customer type, reopened status, and assigned team.

## Dashboard highlights

The supplied dashboard PDF contains five report pages covering:

1.  **Ticket overview and distribution** --- headline ticket KPIs,
    team-wise assignments, category-wise tickets, priority mix, and
    channel-wise customers.
2.  **Resolution analysis** --- resolution hours by issue category,
    priority distribution, and team-wise first-response time.
3.  **City and customer/team mix** --- ticket distribution across cities
    and ratings by assigned team.
4.  **Agent activity** --- agent-wise ticket and customer assignments,
    plus escalated tickets by issue category.
5.  **Customer-level analysis** --- selected-customer ticket details,
    status counts, response/resolution measures, and a written
    observation about response and resolution time.

## Headline figures shown in the dashboard PDF

  Metric                     Dashboard value
  ------------------------ -----------------
  Total tickets                          400
  Tickets in progress                     85
  Pending customers                       57
  Escalated tickets                       27
  Average first response          72 minutes
  Average resolution             36.50 hours
  Reopened tickets                        22
  Total customers                        201

> **Metric validation note:** The dashboard PDF displays an average
> customer rating of **2.06**. A direct average of the nonblank
> `Customer_Rating` values in the supplied Excel sheet is approximately
> **3.70** (222 nonblank ratings). Check the DAX measure, filters, and
> aggregation context in Power BI before publishing or relying on this
> KPI.

## Dataset

The workbook contains two sheets:

-   `Customer_Support_Tickets` --- 400 records with 16 fields.
-   `Day3_Tasks` --- task prompts, suggested visuals, and checks.

Fields in `Customer_Support_Tickets`:

`Ticket_ID`, `Created_Date`, `Resolved_Date`, `Customer_ID`,
`Customer_Type`, `City`, `Channel`, `Issue_Category`, `Priority`,
`Assigned_Team`, `Agent_Name`, `Status`, `Resolution_Hours`,
`First_Response_Minutes`, `Customer_Rating`, `Reopened`.

## Tools and techniques

-   Microsoft Power BI Desktop
-   Power Query for data preparation
-   Data modeling
-   DAX measures
-   Cards, bar/column charts, donut charts, and other report visuals
-   Slicers and interactive filtering

## Dashboard Images 



## Author

**Divyesh Tadvi**\
Power BI \| Data Analytics \| Business Intelligence
