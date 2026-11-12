# Project Details --- Customer Support Ticket Analytics Dashboard

## 1. Project information

  -----------------------------------------------------------------------------------------
  Item                                Details
  ----------------------------------- -----------------------------------------------------
  Project title                       Customer Support Ticket Analytics Dashboard

  Author                              Divyesh Tadvi

  BI tool                             Microsoft Power BI Desktop

  Source workbook                     `Customer_Support_Analytics DATA ONLY.xlsx`

  Dashboard reference                 `CSTD.pdf`

  Dataset size                        400 ticket records

  Number of source fields             16
  -----------------------------------------------------------------------------------------

## 2. Project objective

Analyze customer support ticket data to understand ticket volume and
status, the distribution of issues and priorities, support-channel
usage, team and agent assignments, city-level activity, and response and
resolution times. Present the findings through an interactive Power BI
report.

## 3. Source data structure

The `Customer_Support_Tickets` worksheet contains the following fields:

  Field                      Description based on field name
  -------------------------- ------------------------------------
  `Ticket_ID`                Ticket identifier
  `Created_Date`             Ticket creation date
  `Resolved_Date`            Ticket resolution date
  `Customer_ID`              Customer identifier
  `Customer_Type`            Customer segment/type
  `City`                     Customer/ticket city
  `Channel`                  Support channel
  `Issue_Category`           Ticket issue category
  `Priority`                 Ticket priority
  `Assigned_Team`            Team assigned to the ticket
  `Agent_Name`               Assigned support agent
  `Status`                   Current ticket status
  `Resolution_Hours`         Resolution duration in hours
  `First_Response_Minutes`   First-response duration in minutes
  `Customer_Rating`          Customer rating
  `Reopened`                 Whether the ticket was reopened

The workbook also includes a `Day3_Tasks` worksheet containing analysis
questions, suggested visuals, and checks.

## 4. Dashboard pages and analysis

The supplied PDF has five pages:

### Page 1 --- Customer Support Ticket Analysis

-   Headline ticket and customer KPIs.
-   Team-wise tickets assigned.
-   Category-wise tickets assigned.
-   Priority-wise ticket distribution.
-   Channel-wise customer distribution.
-   Slicers for city, priority, channel, status, issue category,
    reopened status, customer type, and assigned team.

### Page 2 --- Resolution Analysis

-   Resolution hours by issue category.
-   Priority-wise ticket distribution.
-   Team-wise first-response minutes.
-   The same headline KPI context and report filters.

### Page 3 --- City and Ratings Analysis

-   City-wise ticket mix.
-   Ratings and teams mix.
-   Comparison across the cities represented in the report.

### Page 4 --- Agent Analysis

-   Agent list with tickets assigned and customers assigned.
-   Escalated tickets by issue category.
-   Headline KPI context.

### Page 5 --- Customer-Level Analysis

-   Customer ID selection.
-   Selected-customer ticket count and status-related KPIs.
-   Average customer rating, average resolution hours, and average
    first-response minutes.
-   A report note states that average first-response minutes and total
    average resolution hours are positively correlated.
-   The page includes a comparison of CUST-1002 and CUST-1007.

## 5. Dashboard KPIs

The dashboard PDF displays these overall values:

  KPI                         Displayed value
  ------------------------- -----------------
  Total tickets                           400
  Tickets in progress                      85
  Pending customers                        57
  Escalated tickets                        27
  Average first response           72 minutes
  Average resolution              36.50 hours
  Average customer rating                2.06
  Reopened tickets                         22
  Total customers                         201

### Important validation note

The displayed average customer rating needs review before final
publication. In the supplied Excel data, there are 222 nonblank
`Customer_Rating` entries and their direct arithmetic mean is
approximately **3.70**. The dashboard PDF displays **2.06**. These
values are not reconciled here; inspect the Power BI measure,
relationships, filters, and aggregation context to determine why they
differ.

The dashboard's average resolution value is shown as 36.50 hours. The
source workbook has 231 nonblank `Resolution_Hours` values; their direct
mean is approximately 36.50 hours.

## 6. Dataset observations

Counts below are calculated directly from the supplied 400-row
`Customer_Support_Tickets` sheet:

### Tickets by assigned team

  Team                  Tickets
  ------------------- ---------
  Account Services           97
  Delivery Support           87
  Technical Support          86
  General Support            66
  Billing                    64

### Tickets by issue category

  Issue category       Tickets
  ------------------ ---------
  Invoice Request           61
  Payment Issue             59
  Product Question          53
  Account Update            50
  Delivery Delay            48
  Login Problem             45
  Technical Error           43
  Refund Request            41

### Tickets by channel

  Channel       Tickets
  ----------- ---------
  WhatsApp           99
  Web Form           87
  Phone              80
  Live Chat          72
  Email              62

### Tickets by priority

  Priority     Tickets
  ---------- ---------
  Medium           188
  Low               93
  High              89
  Urgent            30

### Tickets by status

  Status               Tickets
  ------------------ ---------
  Resolved                 156
  In Progress               85
  Closed                    75
  Pending Customer          57
  Escalated                 27

### Tickets by city

  City          Tickets
  ----------- ---------
  Vadodara           59
  Ahmedabad          57
  Anand              56
  Rajkot             48
  Mumbai             48
  Bharuch            45
  Surat              45
  Pune               42

## 7. Tools and techniques

The project materials identify/use the following Power BI capabilities
and report elements:

-   Power BI Desktop
-   Power Query / data preparation
-   Data modeling
-   DAX measures
-   KPI cards
-   Bar and column charts
-   Donut charts
-   Slicers and interactive filters
-   Multi-page report navigation and analysis
