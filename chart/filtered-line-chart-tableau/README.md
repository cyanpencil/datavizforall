# Create a Filtered Line Chart with Tableau Public
*by [Veronica X. Armendariz and Jack Dougherty](../../introduction/who.md), last updated March 16, 2017*

An interactive filtered line chart provides checkboxes to turn on/off selected data lines to make specific comparisons, since displaying all of the lines at once would be overwhelming. Readers can float their cursor over each line to identify the school name and data details. We created this tutorial to help a Hartford non-profit education advocacy group compare cohorts of student achievement levels over time across forty schools. You can create your own version with a free downloadable tool for Mac and Windows computers, Tableau Public, https://public.tableau.com

## Try it
<iframe src='https://public.tableau.com/views/LineChartSample/Sheet1?:showVizHome=no&:embed=true' width="90%" height="530"></iframe>

Or right-click the [link to view full-size in a new tab](https://public.tableau.com/views/LineChartSample/Sheet1?:embed=y&:display_count=yes)

## Video with step-by-step tutorial

{%youtube%}_L4u9mfE8Qo{%endyoutube%}

1) Read the [Tableau Public tool review](../tableau-public) in this book, then download and install the free application on a Mac or Windows computer from http://public.tableau.com. Requires a free account.

2) Click link and Save file to download to your computer: [sample-filtered-line-chart in CSV format](https://www.datavizforall.org/chart/filtered-line-chart-tableau/sample-filtered-line-chart.csv). CSV means comma-separated values, a generic spreadsheet format that most data tools can easily open.

Hint: When preparing your own spreadsheet, format your data so that Tableau Public can read it. For example, make sure that Year data is entered as "2007" instead of "1/1/2007". Leave all blank spaces as-is so that Tableau automatically converts them to "null" values during the data import.

3) In Tableau Public, click Connect to import the data file you downloaded to your computer. If you downloaded a CSV file, Connect to Text. Or if you downloaded an Excel file, Connect to Excel. Or click "More..." to connect to Google Sheets.

4) Your data sheet should automatically appear in Tableau Public. Any blanks will automatically convert to “null.”

5) In bottom-left corner, below the "Go to Worksheet" reminder, click Sheet 1.

6) Welcome to the Tableau Public Worksheet. Although it may feel overwhelming at first, the key is learning where to drag-and-drop items from the data tab into the main worksheet. Dimensions are any information that is qualitative or categorical, while measures are quantitative information about the dimensions.  In this example, we are creating a line chart with two dimensions (year and school) and one measure (scores).

7) Drag-and-drop Year into the Column field.

8) Drag-and-drop Schools into the Row field.

9) Drag-and-drop Scores into the middle of the grid.

10) Select Score (but not its drop-down menu), then go to the Analysis menu and turn off Aggregated Measures. We need to do this so that the numbers are displayed individually, and not aggregated by default.

11) In the upper-right corner, go to the Show Me window. (If it is closed, then open it.) Then select Lines (continuous).

12) Initially, each School row appears at its own chart. To blend all of them together into one master chart, drag School to the Marks window and drop it on the Color button. All of the School lines will appear in one chart, with identifying colors.

13) To filter the line chart to display only selected items, go to the Marks window, select the School Cohort drop-down menu, and choose Filter.

14) The Filter window should appear in the far-right side. (If necessary, close the Show Me window to view the Filter window.) Select only a few schools to display by default.

15) Since users can identify schools by turning them on in the Filter window, or floating their cursors to view tooltips for each line, we do not need to show the color legend for each school. In bottom-right School window, select the drop-down menu and choose Hide Card.

16) Confirm or enter text for the axes, title, and caption to describe the data source.

17) To publish your chart on the public web, select File > Save to Tableau Public As. Requires signup for a free Tableau account.

18) Give your workbook a meaningful title, since this name will appear in the URL for your published work on the Tableau Public server, and Save.

19) After publishing your work on the web, Tableau Public will automatically open the web link in your default browser. Click Edit Details to enter more information. Under Toolbar settings, see checkbox to Allow your workbook and its data to be downloaded by others.

![Screenshot: Toolbar settings in Tableau Public](tableau-toolbar-settings-allow.png)

Checking this box enables the Download button at the bottom of your published work, which allows users to access your data and workbook, to see how you constructed the visualization.

![Screenshot: Download button in Tableau Public](tableau-download.png)

20) To insert your Tableau Public visualization in your own website, see the [Embed On Your Web](../../embed/) chapter of this book, and in particular, [Embed Tableau Public on your Website](../../embed/tableau).

21) To see all of your published visualizations, go to your Tableau Public online profile, which follows this format:
```
https://public.tableau.com/profile/USERNAME
```

## Learn more
- Combine multiple visualizations and tell stories with Tableau Public dashboard and story point features. See Tableau Public Resources, with how-to videos and sample data, https://public.tableau.com/en-us/s/resources

{% footer %}
{% endfooter %}
