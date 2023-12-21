
# Phase 3 Code Challenge: Restaurants
Welcome to the Phase 3 Code Challenge for the restaurant review domain. In this assignment, we'll be working with three models: Restaurant, Review, and Customer. These models are interconnected to represent a restaurant review system.

# Topics
SQLAlchemy Migrations
SQLAlchemy Relationships
Class and Instance Methods
SQLAlchemy Querying
Instructions
Before you start coding, take a moment to sketch the domain on paper or a whiteboard. Identify a single source of truth for your data.

# Migrations
You'll need to create migrations for the initial Restaurant and Customer models. Additionally, create a migration for the reviews table with the specified attributes in the deliverables below.

The reviews table should include:

A star_rating column to store an integer.
After creating the necessary tables, use the seeds.py file to create sample instances for testing.

# Deliverables
Write the following methods in the classes, and feel free to build helper methods if needed. Remember to use SQLAlchemy query methods where appropriate.

# Review
Review customer(): Returns the Customer instance for this review.
Review restaurant(): Returns the Restaurant instance for this review.
Restaurant
Restaurant reviews(): Returns a collection of all reviews for the restaurant.
Restaurant customers(): Returns a collection of all customers who reviewed the restaurant.
Customer
Customer reviews(): Returns a collection of all reviews left by the customer.
Customer restaurants(): Returns a collection of all restaurants reviewed by the customer.
Check that these methods work by testing them in the console based on your seed data.

# Aggregate and Relationship Methods
Customer
Customer full_name(): Returns the full name of the customer in Western style (concatenated first and last names).
Customer favorite_restaurant(): Returns the restaurant instance with the highest star rating from this customer.
Customer add_review(restaurant, rating): Creates a new review for the specified restaurant with the given rating.
Customer delete_reviews(restaurant): Removes all reviews for a specific restaurant.
Review
Review full_review(): Returns a string formatted as "Review for {restaurant name} by {customer's full name}: {review star_rating} stars."
Restaurant
Restaurant fanciest() (class method): Returns one restaurant instance with the highest price.
Restaurant all_reviews(): Returns a list of strings with all reviews for this restaurant formatted as specified.
Remember to test these methods in the console using your sample data.

# Notes
This code challenge does not have tests, so ensure your methods work by testing in the console.
Writing working code is prioritized over completing all deliverables.
Refactoring for best practices can be done after ensuring functionality.
Save and run your code before submission to verify it works as expected.
Good luck with the challenge!
