






### 1. Clone repo

```
$ git clone git@github.com:basir/node-react-ecommerce.git
$ cd node-react-ecommerce
```

### 2. Install MongoDB

Download it from here: https://docs.mongodb.com/manual/administration/install-community/

### 3. Run Backend

```
$ npm install
$ npm start
```

### 4. Run Frontend

```
# open new terminal
$ cd frontend
$ npm install
$ npm start
```

### 5. Create Admin User

- Run this on chrome: http://localhost:5000/api/users/createadmin
- It returns admin email and password

### 6. Login

- Run http://localhost:3000/signin
- Enter admin email and password and click signin

### 7. Create Products

- Run http://localhost:3000/products
- Click create product and enter product info

## Support

- Q/A: https://webacademy.pro/oldamazona
- Contact Instructor: [Basir](mailto:basir.jafarzadeh@gmail.com)









In this part, you create a web template for the eCommerce website.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/56kqn8m5n1m9fejdoxkz.png)



We will create a list of products as static HTML elements.



We will create a hamburger menu that shows and hide the sidebar. Also, we design the details page of the products.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/3sceblg6i6790minhaxg.jpg)


This part is about the frontend. We use React library to build the UI elements.



This is the home page of e-commerce. It shows a list of products.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/hqiwteg10o8a2cnq0wwi.jpg)



When the user clicks on a product there should a page to show details about that product. This lesson is all about making an attractive details page.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/csskvzbcmz4ypki2xjgk.jpg)







Shopping Cart is the heart of any e-commerce website. We focus on creating a user-friendly shopping cart using React and Redux.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/fyzf0no5ej1fgxp5972e.png)



We need to register the user before redirecting them to the checkout. In this part, we will create forms for getting user info and save them in the database.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/92coj0rezr5508vhfv34.png)



Admin should be able to define products and update the count in stock whenever they like. This page is about managing ECommerce products.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/154a5zk6vfapukjaxwyu.png)



In this part, we implement the checkout wizard including sign in, shipping info, payment method, and place order.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/l8w3g9mc3ccijt70wpf3.png)


### Part 18- Order Details Screen

It shows all details about an order includeing shipping, payments and order items. Also it is possible for admin to manage orders like set them as delivered.

### Part 19- Connect to PayPal

This parts create PaypalButton component to show paypal payment button on the screen.
when users click on it, they will be redirected to paypal website to make the payment.
after payment users will be redirected to details page of the order.

### Part 20- Manage Order Screen

This is an admin page to manage list of orders. Admin can delete an order or set it as delivered.

### Part 21- User Profile Screen

When user click on thier name on the header menu, this page appears. It consists of two sections. First an profile update form and second order history.

### Part 22- Filter and Sort Products

In the home page, right after header, there is a filter bar to filter products based on their name and description. also it is possible to sort product based on prices and arrivals.

### Part 23- Deploy Website on Heroku

This section explains all steps to publish the ecommerce website on heroku. first you need to create a cloud mongodb and the make an account on heroku.

### Part 24- Rate and Review Products

This part shows list of reviews by users for each products. also it provides a form to enter rating and review for every single product. also it update the avg rating of each product by user ratings.

1. index.html
2. link fontawesome
3. Rating.js
4. create stars based on props.value
5. show text based on props.text
6. index.css
7. style rating, span color gold and last span to gray, link text to blue
8. HomeScreen.js
9. use Rating component
10. ProductScreen.js
11. use Rating component, wrap it in anchor#reviews
12. list reviews after product details
13. create new review form to get rating and reviews
14. index.css
15. style reviews
16. ProductScreen.js
17. implement submitHandler
18. productActions.js
19. create saveProductReview(productId, review)
20. productConstants.js
21. create product review constants
22. productReducers.js
23. create productReviewSaveReducer
24. store.js
25. add productReviewSaveReducer
26. backend
27. productRoute.js
28. router.post('/:id/reviews')
29. save review in product.reviews
30. update avg rating

### Part 25- Upload Product Images On Local Server

Admin shoud be able to uploads photos from their computer. This section is about uploading images on local server ans aws s3 cloud server.

1. npm install multer
2. routes/uploadRoute.js
3. import express and multer
4. create disk storage with Date.now().jpg as filename
5. set upload as multer({ storage })
6. router.post('/', upload.single('image'))
7. return req.file.path
8. server.js
9. app.use('/api/uploads',uploadRoute)
10. ProductsScreen.js
11. create state hook for uploading
12. create input image file and onChange handler
13. define handleUploadImage function
14. prepare file for upload
15. axios post file as multipart/form-data
16. set image and set uploading
17. check result



## Summary

In this tutorial, we have made an eCommerce website like Amazon. Feel free to change this project based on your needs and add it to your portfolio.
