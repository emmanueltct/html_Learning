# AutoMart
Auto Mart is an online marketplace for automobiles of diverse makes, model or body type. With
Auto Mart, users can sell their cars or buy from trusted dealerships or private sellers.

# what a sytem can accomplish
the user visit automart sytem on the home page can view the latest advertised car and click on car image to see details information about car and can buy car if he/she is satisfied or can report car as fraudulent.
# AutoMart UI
	# 1. User can sign up.
	
on the homepage click on signup page and fiil the form data then submit
	# 2. User can sign in.
after making signup you can login into your account through homepage and click on login then fill the form and submit

	# 3. User (seller) can post a car sale advertisement.
after making login on user welcome page  click on publish car and fiil the form data then submit

	# 4. User (buyer) can make a purchase order.
after making login on user welcome page use filter option to see available car then click on details button to see car information if you are satisfied click on purchase button then fill the form and submit  

	# 5. User (buyer) can update the price of his/her purchase order.
on user welcome page click on orders you find list of orders request you have sent and click on new price button of any cary order you want to modify and fill the form then submit 

	# 6. User (seller) can mark his/her posted AD as sold.
on user welcome page click on publishe car you will find the list of car Ad you made and and click on orders button to see which order request have done on specific car then you can mark car as sold by confirming one order request

	# 7. User (seller) can update the price of his/her posted AD.
on user welcome page click on publishe car you will find the list of car Ad you made and and click on deatails button where you find detail information of car the click on update price button fill the form and submit

	# 8. User can view all unsold car .
on user welcome page use fiter option to check all available condition depends on option you have selected

	# 10. Admin can delete a posted AD record.
when you loged in as admin you can delete AD record just see the available record based on unsold car , sold car ,orders and reported car then view details and click on delete button
	# 11. Admin can view all posted ads whether sold or unsold.
On the admin welcome  page use menus and you can see all sold or unsold car

# follow this link  https://emmanueltct.github.io/AutoMart/ 

# API END POINTS

# use postman to test api end points

	# User can sign up.
	POST: http://localhost:3300/api/v1/auth/signup

	# User can sign in
	POST: http://localhost:3300/api/v1/auth/login

	# User (seller) can post a car sale advertisement.
	POST: http://localhost:3300/api/v1/car

	# User (buyer) can make a purchase order
	POST: http://localhost:3300/api/order
	
	# User (buyer) can update the price of his/her purchase order.
	PATCH: http://localhost:3300/api/v1/order/:id/price

	# User (seller) can mark his/her posted AD as sold.
	PATCH: http://localhost:3300/api/v1/car/:id/status

	# User (seller) can update the price of his/her posted AD.
	PATCH: http://localhost:3300/api/v1/car/:id/price

	# User can view a specific car.
	GET: http://localhost:3300/api/v1/car/:id

	# User can view all unsold cars.
	GET: http://localhost:3300/api/v1/car?status=available
	
	# User can view all unsold cars within a price range.
	GET: http://localhost:3300/api/v1/car?status=available&min_price=any price_value&max_price= any price_value
	
	# Admin can delete a posted AD record.
	DELETE: http://localhost:3300/api/v1/car/:id

	# Admin can view all posted ads whether sold or unsold
	GET: http://localhost:3300/api/v1/car

