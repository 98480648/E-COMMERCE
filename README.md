# E-COMMERCE
An E-commerce Web Application with Admin Panel


**AWS EC2 is being used for this project.. Here is the link to the project: http://13.250.198.160:8080/E-Commerce/index.jsp . <br> PS: It is best seen on a desktop browser because it is not responsive..**

# Intro to the project

Here is the application's index page. **Loaded from the database** are all of these products.
<img src="https://github.com/shivamvk/E-Commerce/blob/master/images/Screenshot%20(8).png">

You can click on any item to **view details** like this

<img src="https://github.com/shivamvk/E-Commerce/blob/master/images/Screenshot%20(9).png">

You can also search **search**

<img src="https://github.com/shivamvk/E-Commerce/blob/master/images/Screenshot%20(10).png">

You can add items to your **cart and can checkout** any time

<img src="https://github.com/shivamvk/E-Commerce/blob/master/images/Screenshot%20(11).png">

This is the **admin panel** where you can register and add products after that.
<img src="https://github.com/shivamvk/E-Commerce/blob/master/images/Screenshot%20(12).png">
          
# Install this project on your computer.

**To execute this project on your machine, you must have an Apache-Tomcat server**.
-then create the following mysql tables


desc users;

+----------+-------------+------+-----+---------+----------------+

| Field    | Type        | Null | Key | Default | Extra          |

+----------+-------------+------+-----+---------+----------------+

| userId   | int(11)     | NO   | PRI | NULL    | auto_increment |

| email    | varchar(50) | YES  |     | NULL    |                |

| password | varchar(50) | YES  |     | NULL    |                |

| name     | varchar(50) | YES  |     | NULL    |                |

+----------+-------------+------+-----+---------+----------------+



desc sellers;

+----------+-------------+------+-----+---------+----------------+

| Field    | Type        | Null | Key | Default | Extra          |

+----------+-------------+------+-----+---------+----------------+

| id       | int(11)     | NO   | PRI | NULL    | auto_increment |

| name     | varchar(50) | YES  |     | NULL    |                |

| email    | varchar(50) | YES  |     | NULL    |                |

| password | varchar(50) | YES  |     | NULL    |                |

+----------+-------------+------+-----+---------+----------------+



desc products;

+-----------------------+-------------+------+-----+---------+----------------+

| Field                 | Type        | Null | Key | Default | Extra          |

+-----------------------+-------------+------+-----+---------+----------------+

| productId             | int(11)     | NO   | PRI | NULL    | auto_increment |

| productName           | varchar(50) | YES  |     | NULL    |                |

| productDescription    | varchar(50) | YES  |     | NULL    |                |

| productGender         | varchar(50) | YES  |     | NULL    |                |

| productCategory       | varchar(50) | YES  |     | NULL    |                |

| productQuantitySmall  | int(11)     | YES  |     | NULL    |                |

| productQuantityMedium | int(11)     | YES  |     | NULL    |                |

| productQuantityLarge  | int(11)     | YES  |     | NULL    |                |

| productSoldBy         | varchar(50) | YES  |     | NULL    |                |

| productPrice          | int(11)     | YES  |     | NULL    |                |

| productDiscount       | int(11)     | YES  |     | NULL    |                |

+-----------------------+-------------+------+-----+---------+----------------+



desc cart;

+-----------+-------------+------+-----+---------+-------+

| Field     | Type        | Null | Key | Default | Extra |

+-----------+-------------+------+-----+---------+-------+

| userEmail | varchar(50) | YES  |     | NULL    |       |

| productId | int(11)     | YES  | MUL | NULL    |       |

| size      | varchar(50) | YES  |     | NULL    |       |

+-----------+-------------+------+-----+---------+-------+
