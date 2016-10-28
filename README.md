# d3table
A table written on D3 which takes json as input to load

How to use it
-------------
Step : 1  : Make the html table template
----------------------------------------
  <p>
  <table id="customer_table">
        <thead>
            <tr>
               	<th data-colname="append(firstname,lastname)">Name</th>
               	<th data-colname="phone">phone</th>
				        <th data-colname="status">Status</th>               												                	
            </tr>
        </thead>
    </table>
  </p>
Simply make the table object and call populatedata
--------------------------------------------------
  table().createtable("#customer_table")
				.populatedata(customers)
					.done()

<b><u>Sample Data:</u></b> 
  var customers = [
    { "firstname" : "John", "lastname" : "Miller", "phone" : "111-456-7890", "status": "active" },
    { "firstname" : "Bob", "lastname" : "Wilson", "phone" : "222-456-7890", "status": "active" },
  ];
  
Hope this helps.  
