Welcome to my new dbt project.
I tried to show my skills with dbt and gained benefits from a lot of dbt tools like:
- dbt sources allow you to document those source tables inside a YAML file, where you can reference your source database, the schema, and tables.
- Create some tests to insure the data integrity
- dbt Analyses to store some ad-hoc queries


## In this project, I tried to model a data warehouse living inside AWS RedShift in three stages:

### Staging Layer:
In this layer, I have the data as ingested from OLTP sources and I have 3 models:
- stg_jaffle_shop_customers
- stg_jaffle_shop_orders
- stg_stripe_order_payments

### Intermediate Layer:
in this layer, I only created one model (int_payment_type_amount_per_order)

### Marts Layer
It consists of Data marts that will be used from different department
In this layer, I created a star schema with one fact table and one dimension:
- dim_customers
- fct_orders

## Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [dbt community](https://getdbt.com/community) to learn from other analytics engineers
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
