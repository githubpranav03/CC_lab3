Optimization for /cart:-
In  init .py, a static method in the Product class has been used for loading structured product data, making the code cleaner. Manual loops have been replaced by list comprehensions for efficiency.
Input validation was also introduced for updating product quantities to prevent errors. get_product() was enhanced to handle cases where no product was found.

In dao.py, connection logic has been centralised to a singular reusable connect() function, reducing redundancy. Executemany() has been used for bulk inserts, significantly improving performance during initialization. Using sqlite3.Row allows query results to be accessed as dictionaries, simplifying data handling. CRUD operations have also been optimised.

Optimization for /browse:-
In  init.py, product.load() has been implemented as a static method for better data handling. List comprehensions have been used to make the code more efficient. Input validation has been added to update_qty() for error prevention.

In dao.py, connection logic is being handled by a single reusable connection function to remove redundancy, repetitive insert statements were combined into a single executemany() function.
