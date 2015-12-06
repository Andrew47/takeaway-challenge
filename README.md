# Week 2: Takeaway Challenge

## Installation Requirements

Users must run bundle in the command line to install the required gems for the
program to work.

## Guidance in using the program

First the takeaway must create dishes, giving each a name
and price. An example is provided below:

```ruby
pizza = Dish.new(name: pizza, price: 1)
chicken = Dish.new(name: chicken, price: 2)
```

Note that the labels `name:` and `price:` must be used and both attributes must
be provided. However, the order in which they are provided is not important.

A Dish List can then be created as follows:

```ruby
dish_list = DishList.new(pizza, chicken)
```

The `OrderList` class provides customers with an interface through which to place
orders. Upon creating an order list, customers must specify which dish list the order
will be for. They can determine the prices of different dishes through `price_list`, and
can place their order through `place_order`. If an integer is provided before specifying
the quantities of different dishes ordered, this is interpreted as the customer's expected total
cost. This is used to verify that the order was correctly made, and is optional. 
