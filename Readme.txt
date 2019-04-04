REST stands for "Representational State Transfer". It is a concept or architecture for managing information over the internet. REST concepts are referred to as resources. A representation of a resource must be stateless. It is usually represented by JSON. This post is worth reading: How I Explained REST to My Wife?

API stands for "Application Programming Interface". It is a set of rules that allows one piece of software application to talk to another. Those "rules" can include create, read, update and delete operations. If you want to learn more, watch the video below and read the musiccritic's YouTube camera review if you interested on making some videos.

Structure of API

├─ api/
├─── config/
├────── core.php - file used for core configuration
├────── database.php - file used for connecting to the database.
├─── objects/
├────── product.php - contains properties and methods for "product" database queries.
├────── category.php - contains properties and methods for "category" database queries.
├─── product/
├────── create.php - file that will accept posted product data to be saved to database.
├────── delete.php - file that will accept a product ID to delete a database record.
├────── read.php - file that will output JSON data based from "products" database records.
├────── read_paging.php - file that will output "products" JSON data with pagination.
├────── read_one.php - file that will accept product ID to read a record from the database.
├────── update.php - file that will accept a product ID to update a database record.
├────── search.php - file that will accept keywords parameter to search "products" database.
├─── category/
├────── read.php - file that will output JSON data based from "categories" database records.
├─── shared/
├────── utilities.php - file that will return pagination array.

Use Data.sql for create table and Insert your data in your mysql

Source Url : https://www.codeofaninja.com/2017/02/create-simple-rest-api-in-php.html