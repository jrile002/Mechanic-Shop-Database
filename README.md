# CS166 Project: Mechanic Shop Database
A database system that tracks information about customers, car, mechanics, car ownership, service request and billing information.

## In Progress:
 + **Close A Service Request**: This function will allow you to complete an existing service request. Given a servicerequest number and an employee id, the client application should verify the information provided and attempt to create a closing request record. You should make sure to check for the validity of the provided inputs (i.e. does the mechanic exist, does the request exist, valid closing date after request date, etc.)
 + Have the ID's of customer, mechanic, and service requests automatically increment as opposed to the user putting it in.

## Finished Functions:
 + **Add Customer:** Add a new customer into the database. You should provide an interface that takes customer information (i.e. first, last name, phone, address) as input and checks if the provided information is valid based on the constraints of the database schema.
 + **Add Mechanic:** Add a new mechanic into the database. You should provide an interface that takes as input the information of a new mechanic (i.e. first, last, speciality, experience) and checks if the provided information is valid based on the constraints of the database schema.
 + **Add Car:** This function should allow a new car to be added in to the database. You should provide an interface that takes as input the information of a new car (i.e. vin, make, model, year) checking if the provided information is valid based on the constraints of the database schema.
 + **Initiate a Service Request:** This function will allow you to add a service request for a customer into the database. Given a last name, the function should search the database of existing customers. If many customers match, a menu option should appear listing all customers with the given last name asking the user to choose which customer has initiated the service request. Otherwise, the client application should provide the option of adding a new customer. If an existing customer is chosen, the client application should list all cars associated with that client providing the option to initiate the service request for one of the listed cars, otherwise a new car should be added along with the service request information for it. 
 + **List date, comment, and bill for all closed requests with bill lower than 100.** List the customers that have paid less than 100 dollars for repairs based on their previous service requests. 
 + **List first and last name of customers having more than 20 different cars.** 
Find how many cars each customer has counting from the ownership relation and discover who has more than 20 cars. 
 + **List Make, Model, and Year of all cars build before 1995 having less than 50000 miles.** Get the odometer from the service_requests and find all cars before 1995 having less than 50000 miles in the odometer. 
 + **List the make, model and number of service requests for the first k cars with the highest number of service orders.** Find for all cars in the database the number of service requests. Return the make,
model and number of service requests for the cars having the k highest number of
service requests. The k value should be positive and larger than 0. The user should
provide this value. Focus on the open service requests.
 + **List the first name, last name and total bill of customers in descending order of their total bill for all cars brought to the mechanic.** For all service requests find the aggregate cost per customer and order customers according to that cost. List their first, last name and total bill.
