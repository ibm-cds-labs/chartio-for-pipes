# Creating a Chart


## Overview
This tutorial will walk you through creating your first chart in Chartio. In just a few minutes,
you'll be visualizing the top 5 delinquent customers by plan amount based on Stripe invoice data
stored in dashDB! Before starting this tutorial, make sure you have completed the
[Getting Connected tutorial](../getting-connected/README.md). Don't hesitate to
[contact support](../support/README.md) if you run into any issues!


## Tutorial

### Steps
- [Create a new dashboard, name it, categorize it and click "Create Dashboard"](#create-a-new-dashboard-name-it-categorize-it-and-click-create-dashboard)
- [Navigate to the Chart Creator by adding a Chart element](#navigate-to-the-chart-creator-by-adding-a-chart-element)
- [Search for the `St Customer` table](#search-for-the-st-customer-table)
- [Drag `Email` into Diemnsions and `Delinquent` into Filters, filter on "equals 1"](#drag-email-into-diemnsions-and-delinquent-into-filters-filter-on-equals-1)
- [Drag `Plan Amount` from `St Customer Subscriptions` into Measures, sort descending](#drag-plan-amount-from-st-customer-subscriptions-into-measures-sort-descending)
- [Limit the result set to 5 and click "Refresh Chart"](#limit-the-result-set-to-5-and-click-refresh-chart)
- [Use the Data Pipeline to divide the `Plan Amount` in cents by 100 to get dollars](#use-the-data-pipeline-to-divide-the-plan-amount-in-cents-by-100-to-get-dollars)
- [Change the visualization from table to bar chart](#change-the-visualization-from-table-to-bar-chart)
- [Navigate to the Chart Settings, title the chart and y-axis and click "Done"](#navigate-to-the-chart-settings-title-the-chart-and-y-axis-and-click-done)
- [Save the chart to the dashboard](#save-the-chart-to-the-dashboard)

### Create a new dashboard, name it, categorize it and click "Create Dashboard"
![Create a new dashboard](./img/00-new-dashboard.png)
![Name and categorize the dashboard and click "Create Dashboard"](./img/01-dashboard-settings.png)

### Navigate to the Chart Creator by adding a Chart element
![Add a Chart Element](./img/02-new-element.png)
![The Chart Creator](./img/03-chart-creator.png)

### Search for the `St Customer` table
![Search for the `St Customer` table](./img/04-metadata-search.png)

### Drag `Email` into Diemnsions and `Delinquent` into Filters, filter on "equals 1"
![Drag `Email` into Diemnsions and `Delinquent` into Filters, filter on "equals 1"](./img/05-st-customer.png)

### Drag `Plan Amount` from `St Customer Subscriptions` into Measures, sort descending
![Wait for success notification and check the Schema tab](./img/06-st-customer-sub.png)

### Limit the result set to 5 and click "Refresh Chart"
![Limit the result set to 5 and click "Refresh Chart"](./img/07-limit.png)

### Use the Data Pipeline to divide the `Plan Amount` in cents by 100 to get dollars
![Use the Data Pipeline to divide the `Plan Amount` in cents by 100 to get dollars](./img/08-edit-column.png)

### Change the visualization from table to bar chart
![Change the visualization from table to bar chart](./img/09-bar-chart.png)

### Navigate to the Chart Settings, title the chart and y-axis and click "Done"
![Navigate to the Chart Settings](./img/10-chart-settings.png)
![Add a chart title](./img/11-chart-title.png)
![Add a y-axis title and click "Done"](./img/12-axis-title.png)

### Save the chart to the dashboard
![Save the chart to the dashboard](./img/13-save-chart.png)
![View it on the dashboard](./img/14-dashboard.png)
