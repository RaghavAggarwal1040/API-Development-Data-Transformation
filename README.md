# API Development and Data Transformation

Objective: The objective of this assignment is to develop APIs, using the attached dataset, of
purchases of different softwares through out the year. Candidates are free to use the dataset
directly or import it in any database, if importing , make sure to include a migration file or
readme steps so that we can run and check the APIs ourselves.


## Dataset Source

### Card transaction data: 
https://drive.google.com/file/d/1YfhCPZbofAekMy9tPH_7ZXChVX8w_OUF/view?usp=sharing


## Requirements.txt

Install the follwoing files in remote server.
- flask (Flask, jsonify, request)
- pandas
- json
## Tasks

#### Api 1
 - End point : /api/total_items 
 - API Use Cases :
   - Total item (total seats) sold in Marketting for last in q3 of the year?
   - Expected O/P: returns integer
   - Parameters: {start_date: DATE, end_date: DATE, department: string}

Link : http://127.0.0.1:5000/api/total_items?start_date=2022-07-01&end_date=2022-09-30&department=Marketting

![image_2023_06_24T03_35_35_074Z](https://github.com/RaghavAggarwal1040/API-Development-Data-Transformation/assets/66468678/9e873b3e-ae0e-4f46-80c2-fc947849cfae)



#### Api 2
 - End point : /api/nth_most_total_item 
 - API Use Cases :
   -  What is the 2nd most sold item in terms of quantity sold in q4?
   -  What is the 4th most sold item in terms of Total price in q2?
   - Expected O/P: returns string name
   - Parameters: { item_by: ("quantity" | | "price"), start_date: DATE, end_date:DATE, n:integer }

Link : http://127.0.0.1:5000/api/nth_most_total_item?item_by=quantity&start_date=2022-10-01&end_date=2022-12-31&n=2
![image_2023_06_24T03_38_00_157Z](https://github.com/RaghavAggarwal1040/API-Development-Data-Transformation/assets/66468678/948a33d6-8c20-4660-8282-80a02f1cd2ed)

Link : http://127.0.0.1:5000/api/nth_most_total_item?item_by=price&start_date=2022-10-01&end_date=2022-12-31&n=2

![image_2023_06_24T03_38_54_982Z](https://github.com/RaghavAggarwal1040/API-Development-Data-Transformation/assets/66468678/b6b4bcd0-6381-4a67-accc-6c68e1f24ef2)



#### Api 3
  - End point : /api/percentage_of_department_wise_sold_items
  - API Use Cases:
    - What is the percentage of sold items (seats) department wise?
    - Expected O/P: {dept_name: x%,……. }
    - Parameters: {start_date: Date, end_date: Date}

Link : http://127.0.0.1:5000/api/percentage_of_department_wise_sold_items?start_date=2022-01-01&end_date=2022-12-31

![image_2023_06_24T03_41_06_810Z](https://github.com/RaghavAggarwal1040/API-Development-Data-Transformation/assets/66468678/02a5d5a3-7779-4a59-98c2-7ccfb3748623)



#### Api 4

  - End point : /api/monthly_sales
  - API Use Cases:
      - How does the monthly sales for any product look like?
      - Expected O/P: [1908.0, … 1952.0] for all 12 months
      - Parameters: {product: String, year:Number}

Link :  http://127.0.0.1:5000/api/monthly_sales?product=Outplay&year=2022
![image_2023_06_24T03_43_39_816Z](https://github.com/RaghavAggarwal1040/API-Development-Data-Transformation/assets/66468678/a59c36b8-6335-4eac-b75c-284df37ed17a)


## Feedback

If you have any feedback, please reach out at raghav.aggarwal2001@gmail.com || https://raghavaggarwalportfolio.netlify.app/


