============Steps to run the Rest api =============

1) Import MyRetail SpringBoot project into workspace.

2) Maven clean 

    Select MyRetail --> Run As --> Maven clean

3) Update MyRetail Project 
   
     Select MyRetail --> Maven --> Update project
     
4) Run as Java application MyRetailApplication.java 

5) To goto H2 database 
      
       http://localhost:8080/h2-console
  
6) Add the values to the MY_RETAIL H2-Database.
	example:
		  	ID  		   CURRENCY_CODE   CURRENT_PRICE  		P_NAME  
			16551552	       INR			       	19				    pevari
			13860428		     USD				      102				    Big lebowski
			
7) use postman to do the following:

	a)to get all the product details
	      GET request-> http://localhost:8080/product/
	
	b)to get particular product details
	      GET request-> http://localhost:8080/product/id
	
	c)to create product
	      POST request->http://localhost:8080/product
	      add JSON format data into body test 
	
                        example:
                      {
                            "id": 1,
                            "p_name": "Shankar",
                            "current_price": 100,
                            "currency_code": "INR"
                        }
    
    d)to delete particular product
          DELETE request-> http://localhost:8080/product/id
    
    BONUS TASK:
    
    e)to update particular product price by id
          PUT request-> http://localhost:8080/product/id
    
                        example:
                        {
                            "id": 1,
                            "p_name": "Shankar",
                            "current_price": 500,    #here price is updated
                            "currency_code": "INR"
                        }


	
