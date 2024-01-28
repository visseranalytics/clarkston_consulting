# Clarkston Consulting Interview Assignment

Scenario: A consumer-packaged goods company is migrating Customer Master Data to a new SAP entity from a LEGACY system. You are a member of the Data Migration Team and responsible for completing the transformation component of the overall ETL process. You have been provided with an extract of the customer records and technical spec on the transformation that should occur.

The requirement is to build a transformation layer utilizing Jupyter notebook(s):

<ol>
<li>Reads in the CustomerExtract.csv</li>
<li>Completes an initial profile of the data and performs data quality checks that you think are needed e.g. Are there any fields in the extract that are populated with data that are not flagged in the spec (Field Utilized in LEGACY System)<ol><li>Quality checks should be visible in the notebook and output for traceability</li></ol></li>
<li>Cleanup any data quality issues, such as special characters in the Name 1 field</li>
<li>Perform the transformations included in the spec</li>
<li>Output a flat file named CustomerLoad.csv</li>
</ol>

This file will be used by another member of the project team to load the data in the new SAP entity. 


About this assignment:
<ol>
<li>You should use a Jupyter notebook(s) to complete this assignment. In the notebook please include markdown for general documentation and comment out any data analysis done as part of this exercise.</li>
<li>After completion, please package in a way that will be easy for the recipient to install/check the code package.  You may use GitHub if you want.</li>
<li>Please send the code/assignment to the recruitment coordinator at least 24 hours before your final interview.</li>
</ol>


# My Process

<ul>
<li>Convert the spec into a usable format</li>
<li>Rename the extract fields with friendly labels from spec</li>
<li>Check for any issues in the extract such as truncation, bad types, missing fields, etc</li>
<li>Remove special characters from the string fields.</li>
</ul>


# Found Problems (Fixed By Filtering To Used Fields)

<ul>
    <li>Account Group and Customer Account have ambiguous field names in the extract. There are two fields in the spec with distinct table/column name combos but the extract doesn't specify which is which.</li>
    <li>Duplicate SAP Field Descriptions</li>
    <li>Leading and trailing special characters for the field descriptions. This is only an issue due to converting the field names in the extract to friendly terms</li>
</ul>