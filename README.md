## Problem Statement:
Assume you are a data analyst/scientist at **Target** and are assigned the task of analyzing the given dataset to extract valuable insights and provide actionable recommendations.

---

## Context:
**Target** is a globally renowned brand and a prominent retailer in the United States. It makes itself a preferred shopping destination by offering outstanding value, inspiration, innovation, and an exceptional guest experience.

This business case focuses on **Target’s operations in Brazil** and provides information about 100,000 orders placed between 2016 and 2018. The dataset offers a comprehensive view of various dimensions, including:
- **Order Status**
- **Price**
- **Payment and Freight Performance**
- **Customer Location**
- **Product Attributes**
- **Customer Reviews**

Analyzing this extensive dataset can provide insights into:
- Order processing
- Pricing strategies
- Payment and shipping efficiency
- Customer demographics
- Product characteristics
- Customer satisfaction levels

---

## Dataset:
The data is available in **8 CSV files**:
- `customers.csv`
- `sellers.csv`
- `order_items.csv`
- `geolocation.csv`
- `payments.csv`
- `reviews.csv`
- `orders.csv`
- `products.csv`

---

### **Customers Dataset (`customers.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `customer_id`               | ID of the consumer who made the purchase          |
| `customer_unique_id`        | Unique ID of the consumer                         |
| `customer_zip_code_prefix`  | Zip Code of the consumer’s location               |
| `customer_city`             | Name of the city from where the order is made     |
| `customer_state`            | State Code from where the order is made (e.g., SP)|

---

### **Sellers Dataset (`sellers.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `seller_id`                 | Unique ID of the seller registered                |
| `seller_zip_code_prefix`    | Zip Code of the seller’s location                 |
| `seller_city`               | Name of the city of the seller                    |
| `seller_state`              | State Code (e.g., SP)                             |

---

### **Order Items Dataset (`order_items.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `order_id`                  | Unique ID of the order made by consumers          |
| `order_item_id`             | Unique ID given to each item in the order         |
| `product_id`                | Unique ID of each product available on the site   |
| `seller_id`                 | Unique ID of the seller                           |
| `shipping_limit_date`       | Date before which the product must be shipped     |
| `price`                     | Actual price of the ordered products              |
| `freight_value`             | Price rate for product delivery                  |

---

### **Geolocation Dataset (`geolocation.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `geolocation_zip_code_prefix`| First 5 digits of the Zip Code                   |
| `geolocation_lat`           | Latitude                                         |
| `geolocation_lng`           | Longitude                                        |
| `geolocation_city`          | City                                             |
| `geolocation_state`         | State                                            |

---

### **Payments Dataset (`payments.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `order_id`                  | Unique ID of the order                           |
| `payment_sequential`        | Sequences of payments for EMI transactions       |
| `payment_type`              | Mode of payment used (e.g., Credit Card)         |
| `payment_installments`      | Number of installments for EMI purchases         |
| `payment_value`             | Total amount paid for the order                  |

---

### **Orders Dataset (`orders.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `order_id`                  | Unique ID of the order                           |
| `customer_id`               | ID of the consumer who made the purchase         |
| `order_status`              | Status of the order (e.g., delivered, shipped)   |
| `order_purchase_timestamp`  | Timestamp of the purchase                        |
| `order_delivered_carrier_date` | Delivery date at which the carrier made the delivery |
| `order_delivered_customer_date` | Date when the customer received the product    |
| `order_estimated_delivery_date` | Estimated delivery date                      |

---

### **Reviews Dataset (`reviews.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `review_id`                 | ID of the review given on the product            |
| `order_id`                  | Unique ID of the order                           |
| `review_score`              | Review score given by customers (1-5 scale)      |
| `review_comment_title`      | Title of the review                              |
| `review_comment_message`    | Comments posted by the consumer                  |
| `review_creation_date`      | Timestamp when the review was created            |
| `review_answer_timestamp`   | Timestamp when the review was answered           |

---

### **Products Dataset (`products.csv`)**
| **Feature**                  | **Description**                                   |
|------------------------------|--------------------------------------------------|
| `product_id`                | Unique ID of the product                         |
| `product_category_name`     | Name of the product category                     |
| `product_name_lenght`       | Length of the product name string                |
| `product_description_lenght`| Length of the product description                |
| `product_photos_qty`        | Number of product photos available               |
| `product_weight_g`          | Weight of the product in grams                   |
| `product_length_cm`         | Length of the product in centimeters             |
| `product_height_cm`         | Height of the product in centimeters             |
| `product_width_cm`          | Width of the product in centimeters              |


## Dataset schema:

![Alt text](https://lh6.googleusercontent.com/ps0KE3yQqTKCax3okKC1E_A8XZ5HF7-B-ur36wk2pgoCpSEidBkUglQOpJ_K8XubsOrxR7aavukqYrZaSL1KcYUk4W4fpjdmdXjIW8dZ9Jh2zekC74LroDR90kJnE0pZk56mytqMfvxbd08PdA)
