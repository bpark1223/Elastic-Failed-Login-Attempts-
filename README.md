# SIEM Visualization of Failed Login Attempts
Creating a dashboard and visualizations 

1. Log into Elastic and click on "dashboard" by way of the side navigation toggle. Then, click "create new dashboard"
<img width="1428" alt="Screenshot 2024-06-24 at 9 51 32 PM" src="https://github.com/bpark1223/Elastic-Failed-Login-Attempts-/assets/77799235/2fdaf8cb-afb9-4105-aadd-88fc51a4252e">
</p>
2. Click "create visualization"
<img width="1440" alt="Screenshot 2024-06-24 at 10 42 15 PM" src="https://github.com/bpark1223/Elastic-Failed-Login-Attempts-/assets/77799235/9d1a75e7-0b43-4bd5-b2bc-de967d900300">
</p>
3. The next page will display several things:
</p>
<pre>  - Filter option before creating a graph (specify field, operator, and value) </pre>
<pre>  - Data set (index) that will be used for the visualization (Windows, Linux, network, etc.)  </pre>
<pre>  - Search bar for checking for a specific field within the data set </pre>
<pre>  - Drop-down menu enabling us to select the type of visualization we want to create (default is "bar vertical stacked", but I will be going with the "table" option) </pre>
<img width="1440" alt="Screenshot 2024-06-24 at 10 13 04 PM" src="https://github.com/bpark1223/Elastic-Failed-Login-Attempts-/assets/77799235/096365b5-eb1a-48cf-95bf-065a7c3044ca">
</p>
4. Under "table" is the "rows" section where I choose the specific data elements to include in the table view. The field I chose is "user.name.keyword" 
<img width="1429" alt="Screenshot 2024-06-24 at 10 20 55 PM" src="https://github.com/bpark1223/Elastic-Failed-Login-Attempts-/assets/77799235/b4fc75dc-11c1-4d49-bbc9-323563cf1fb8">
</p> 5. Under the "rows" section is the "metrics" section, where I will use count as the given metric. </p>
<img width="1420" alt="Screenshot 2024-06-24 at 10 28 13 PM" src="https://github.com/bpark1223/Elastic-Failed-Login-Attempts-/assets/77799235/38e95899-47b3-4449-b8e9-fb136af4192d">
</p> 6. Add another row to show the machine where the failed logon attempt occurred. I will add a host.hostname.keyword field, which represents the computer reporting the failed logon attempt, whcih will allow us to display the hostname or machine name alongside the count of failed logon attempts. Now we can see three columns in the table, which contain the following information: </p>

<pre>  - The username of the individuals logging in) </pre>
<pre>  - he machine on which the logon attempt occurred </pre>
<pre>  - The number of times the event has occurred </pre>
<img width="1254" alt="Screenshot 2024-06-24 at 10 51 36 PM" src="https://github.com/bpark1223/Elastic-Failed-Login-Attempts-/assets/77799235/c21101ad-cad1-4c21-8b90-2d023a5752e3">
</p> 7. click on "Save and return", and you will observe that the new visualization is added. save dashboard as well. </p>






