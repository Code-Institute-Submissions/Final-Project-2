# Ayurvedic Store
## Agenda
This webpage enables the user to shop online their needs in a Ayurvedic store.
## Typographic
The color and fonts have been selected to suit the agenda of the website. Aimed at having colors and font that are pleasant,clear and readable for the users to explore the site and make purchase in our website.
### UX Design
The initial idea of the website and its ux Design has been created in Wireframe.
### User Stories
 #### Customer
-  Customer  should be able to browse the products based on ,
    - Catergory
    - Price
    - Rating
- Customer be able to search the product with the keyword.
- Customer be able to sort the products in ascending or descending by name, price,rating.
- Customer be able to view product details and photo.
- Customer be able to add items to the cart.
- Customer be able to adjust or delete items from the bag.
- Customer be able to create an account and login to it.
- Customer can update their personal details.
- Customer can checkout as a guest.
- Pay with credit card.
- Enter shipping  address.

#### Admin
- Admin be able to add procucts.
- Admin be able to edit or delete products.
- Admin be able to see the user details.

### Features
#### Existing Features
 - Header allows users to see the webpage name and also to navigate to different pages of the website.
 - Header contains search box to search entire site.
 - Header allows the user to browse through the products.
 - Products pag the user can see the lsit of products and also on clicking a product thats the user to a product details page.
 - Product details page the user can view and read the product picture and decription.
 - User can add a product to the shopping bag
 - Shoping bag pag allows user to alter the quanity of item or remove the item.
- Register option in the header allows the user to create an account.
- Login option allows the user to login to their account.
- Once registeration is done , an email is send for the user to confirm the registertion.
- Checkout can be done by making card payment.
- Confirmation mail on the purchase will be sent to the customer.
#### Future Features
- Social media login
- User to provide ratings
### Technologies Used
#### List of technologies Used
- HTML
- CSS
- JavaScript
- Python
- Django
- Bootstrap
- JQuery
- Gunicorn
- Psycopg2
- Stripe
- Gitpod
- Github
- Herokku
- AWS S3 bucket
- Balsamiq
- SQlite3
- PostgreSQL
### Testing
#### Header Section
##### Test cases for desktop view
 - Company name should appear on the header.
 - Nav bar should apprar with all its link functioning as expected.
 - Menu options should be displayed horizontally in the header.
 - A search box must be seen in the header.
 - User should be able to see my account and shopping cart options.
 - When clicked the alll products option a dropdown menu with optionslike by catergories, by rating, by price should be visible.
 - Search result must be provided when searched by keyword in the search box.
 - My account when clicked should show the dropdown options of login or register.
 - When clicked register , the user should be able to create an account.
 - User should be get a confirmation mail for creating account.
 - When user should be able to login using their username and password.
 - Once te user logged in and successfully logged in message with the username should be displayed.
 - The cart should always display the grant total of the shopping bag.


##### Test cases for mobile view
- Company name should appear on the header.
- Nav bar should collapse to the burger button with pulldown menu option should appear.
- Menu options should be displayed vertically in the header.
- A search box must be seen in the header.
- User should be able to see my account and shopping cart options.
- When clicked the alll products option a dropdown menu with optionslike by catergories, by rating, by price should be visible.
- Search result must be provided when searched by keyword in the search box.
- My account when clicked should show the dropdown options of login or register.
- User should be get a confirmation mail for creating account.
- When user should be able to login using their username and password.
- Once te user logged in and successfully logged in message with the username should be displayed.
- The cart should always display the grant total of the shopping bag.
#### Home page

##### Test cases for Desktop view
- User should be able to see the welcome message.
- when shop now button is clicked takes to product page.
##### Test cases for Mobile view
- User should be able to see the welcome message.
- when shop now button is clicked takes to product page.

#### Product page
##### Test cases for Desktop view
- User to be able to view products name, image if available..
- when clicked on the product ,it must take to the respective product detail page.
- Product detail page the user can add the product to shopping bag when clicked add to cart.
- User should be able to continue the shopping when clicked keep shopping.
- User must see a notification about their addition of items in the shopping bag.
##### Test cases for mobile view
- User to be able to view products name, image if available.
- when clicked on the product ,it must take to the respective product detail page.
- Product detail page the user can add the product to shopping bag when clicked add to cart.
- User should be able to continue the shopping when clicked keep shopping.
- User must see a notification about their addition of items in the shopping bag.
#### Shopping cart 
##### Test cases for Desktop view
- User should be able to see the items image, name and the quanity subtotal andgrant total.
- user shold be able to adjust the quantity of the item.
- User should be able to see the keep shopping and secure checkout buttons.
- when clicked the keep shopping button , the user should be able to continue shopping.
- when clicked the checkout the user should be taken to the checkout page.
##### Test cases for Mobile view
- User should be able to see the items image, name and the quanity subtotal andgrant total.
- user shold be able to adjust the quantity of the item.
- User should be able to see the keep shopping and secure checkout buttons.
- when clicked the keep shopping button , the user should be able to continue shopping.
- when clicked the checkout the user should be taken to the checkout page.
#### Checkout Page
##### Test cases for desktop view
- User should be able to see a to be filled form asking for shipping address.
- if the user is logged in , he must be able to see his name and details pre filled.
- User should be able to fill in card details  and complete shopping.
- User should receive a mail with the order details to the email id they provided during login.

##### Test cases for mobile view
User should be able to see a to be filled form asking for shipping address.
- if the user is logged in , he must be able to see his name and details pre filled.
- User should be able to fill in card details  and complete shopping.
- User should receive a mail with the order details to the email id they provided during login.

#### Deployment
##### Deployment in Github
1. Go to Final-project Github Repository.
2. Click on Code beside Gitpod.
3. A drop down menu open then click on Download Zip
4. Unzip the downloaded zip file.
5. Install all requirements from the requirements.txt file putting this command into your terminal:
pip3 install -r requirements.txt
7. In the terminal in your IDE migrate the models to create a database using the following commands:
python3 manage.py makemigration, python3 manage.py migrate
8. Load the data fixtures(categories, products, itinerary, itinerary_items, events) in that order into the database using the following command:
python3 manage.py loaddata <fixture_name>
9. Create a superuser to have an access to the the admin panel(you need to follow the instructions then and insert username,email and password):
python3 manage.py createsuperuser
10. You will now be able to run the application using the following command:
python3 manage.py runserver
11. To access the admin panel, you can add the /admin path at the end of the url link and login using your superuser credentials.

#### Heroku Deployment
1. Created a Heroku account @ https://signup.heroku.com/
2. Create requirements.txt file in Gitpod workspace for Heroku to understand installation files to run app. From CLI type type pip3 freeze --local > requirements.txt.
3. To install the Heroku command line on Gitpod, use the following command npm install -g heroku
4. Create a new app with apropriate title and server in Heroku. This creates a connection between the Gitpod application and Heroku that would allow us to push our changes using Git to update the application at any given time.
5. To login to Heroku from the CLI, use the command heroku login
6. To get the application up and running a Procfile is required that istructs Heroku which file is the entry point. Use the following command to create this: echo web: python app.py
7. Code that is prepared to be pushed from Github to Heroku can be executed following the CLI commands: git add . git commit -m "fist Heroku commit" git push
8. Now that the relevant code is pushed to Github, it can also be pushed to Heroku from the chosen branch (e.g. Master)
9. To connect an existing repository from Github to Heroku use the following CLI syntax: heroku git:remote -a [followed by name of Heroku app]
10. To push to Heroku Master Branch, then simply use git push heroku master
11. To scale dynos and run the app in Heroku, use the CLI command: heroku ps:scale web=1
12. In order for the server instance on Heroku to know how to run our application, we need to specify a few Config Vars in Heroku. To do this go to Settings tab > Config Variables and input: AWS_ACCESS_KEY_ID; AWS_SECRET_ACCESS_KEY; DATABASE_URL; DISABLE_COLLECTSTATIC; EMAIL_ADDRESS; EMAIL_PASSWORD EMAIL_PASSWORD; SECRET_KEY; STRIPE_PUBLISHABLE; STRIPE_SECRET.
13. The following syntax will need to be added to your settings.py file to access the SECRET KEY for the new database URL DATABASES = {'default': dj_database_url.parse(os.environ.get('DATABASE_URL'))}
14. The Database can then be migrated to the Heroku Postgres (postgresql) database using the the commands mmakemigrations and migrate from the command line.
15. Once the build in Heroku is complete, click the Open app button.
16. Objects can then be added to the new postgres database using the Admin Panel and logging in with your superuser credentials.
 #### Credits
1. The images and products are used only for educaational purpose and not for any commerical use.

