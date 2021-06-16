

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












![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/56kqn8m5n1m9fejdoxkz.png)




![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/3sceblg6i6790minhaxg.jpg)



![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/hqiwteg10o8a2cnq0wwi.jpg)




![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/csskvzbcmz4ypki2xjgk.jpg)






![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/fyzf0no5ej1fgxp5972e.png)




![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/92coj0rezr5508vhfv34.png)



![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/154a5zk6vfapukjaxwyu.png)


![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/l8w3g9mc3ccijt70wpf3.png)


### - Order Details Screen

It shows all details about an order includeing shipping, payments and order items. Also it is possible for admin to manage orders like set them as delivered.

### -Connect to PayPal

This parts create PaypalButton component to show paypal payment button on the screen.
when users click on it, they will be redirected to paypal website to make the payment.
after payment users will be redirected to details page of the order.



