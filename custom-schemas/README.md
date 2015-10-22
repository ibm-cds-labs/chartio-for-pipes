# Custom Schemas


## Overview
This tutorial will walk you through creating team-specific custom schemas within Chartio. In the
[Getting Connected tutorial](../getting-connected/README.md), we created a connection to dashDB and
imported *all* of the available tables from both Salesforce and Stripe. This is great for admin or
power users but can be dificult to navigate for departmental teams who only need access to a portion
of the tables to do their job. To address this issue we will create two team-specific schemas:

- **dashDB Finance:** This will limit access to just the Stripe data. For convenience, it will also
                      include a custom column that converts an amount stored in Stripe as cents to
                      dollars.
- **dashDB Sales:** This will limit access to just the Salesforce data. For convenience, it will
                    also include a custom table that limits access further to just

Before starting this tutorial, make sure you have completed the
[Creating a Chart tutorial](../creating-a-chart/README.md) in order to fully understand the value of
creating custom schemas. Also, [contact support](../support/README.md) to get two additional clones
of the dashDB Admin data source we set up in the
[Getting Connected tutorial](../getting-connected/README.md). In lieu of contacting support, you
could also go through the steps in the [Getting Connected tutorial](../getting-connected/README.md)
two additional times. The end result should be two new data sources as follows:

![dashDB Finance](./img/00-dashdb-finance.png)
![dashDB Sales](./img/01-dashdb-sales.png)


## Tutorial

### Steps
- [Hide all tables in the dashDB Finance data source](#hide-all-tables-in-the-dashdb-finance-data-source)
- [Toggle visibility on for the `St` prefixed tables (except for overflow system tables)](#toggle-visibility-on-for-the-st-prefixed-tables-except-for-overflow-system-tables)
- [Create a `Plan Amount ($)` custom column on the `St Customer Subscription Data` table](#create-a-plan-amount--custom-column-on-the-st-customer-subscription-data-table)
- [Set the Query Mode to "Interactive Mode Only" on the General tab](#set-the-query-mode-to-interactive-mode-only-on-the-general-tab)
- [Click "Explore" and create a chart with the new `Plan Amount ($)` custom column](#click-explore-and-create-a-chart-with-the-new-plan-amount--custom-column)
- [Hide all tables in the dashDB Sales data source](#hide-all-tables-in-the-dashdb-sales-data-source)
- [Toggle visibility on for the `Sf` prefixed tables (except for overflow system tables)](#toggle-visibility-on-for-the-sf-prefixed-tables-except-for-overflow-system-tables)
- [Create a `Open Opportunities` custom table](#create-a-open-opportunities-custom-table)
- [Set the Query Mode to "Interactive Mode Only" on the General tab](#set-the-query-mode-to-interactive-mode-only-on-the-general-tab-1)
- [Click "Explore" and create a chart with the new `Open Opportunities` custom table](#click-explore-and-create-a-chart-with-the-new-open-opportunities-custom-table)

### Hide all tables in the dashDB Finance data source
![dashDB Finance hide all](./img/02-dashdb-finance-hide-all.png)
![dashDB Finance hide all result](./img/03-dashdb-finance-hide-all-result.png)

### Toggle visibility on for the `St` prefixed tables (except for overflow system tables)
![dashDb Finance toggle visibility](./img/04-dashdb-finance-toggle.png)

### Create a `Plan Amount ($)` custom column on the `St Customer Subscription Data` table
![Add custom column](./img/05-add-custom-column.png)
![Plan Amount $](./img/06-plan-amount-$.png)
![Add column](./img/07-add-column.png)

### Set the Query Mode to "Interactive Mode Only" on the General tab
![dashDB Finance interactive mode only](./img/08-dashdb-finance-interactive-mode.png)

### Click "Explore" and create a chart with the new `Plan Amount ($)` custom column
![Click "Explore"](./img/09-dashdb-finance-explore.png)
![Plan Amount $ chart](./img/10-plan-amount-$-chart.png)

### Hide all tables in the dashDB Sales data source
![dashDB Sales hide all](./img/11-dashdb-sales-hide-all.png)
![dashDB Sales hide all result](./img/12-dashdb-sales-hide-all-result.png)

### Toggle visibility on for the `Sf` prefixed tables (except for overflow system tables)
![dashDb Finance toggle visibility](./img/13-dashdb-sales-toggle.png)

### Create a `Open Opportunities` custom table
![Add custom column](./img/14-add-custom-table.png)
![Plan Amount $](./img/15-open-opps.png)

### Set the Query Mode to "Interactive Mode Only" on the General tab
![dashDB Finance interactive mode only](./img/16-dashdb-sales-interactive-mode.png)

### Click "Explore" and create a chart with the new `Open Opportunities` custom table
![Click "Explore"](./img/17-dashdb-sales-explore.png)
![Plan Amount $ chart](./img/18-open-opps-chart.png)
