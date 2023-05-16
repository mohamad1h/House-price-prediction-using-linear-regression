# House-price-prediction-using-linear-regression
This code is a solution to the hackerrank problem: Multiple Linear Regression: Predicting House Prices


Problem:
Objective
In this challenge, we practice using multiple linear regression to predict housing prices. Check out the Resources tab for helpful videos!

Task
Charlie wants to buy a house. He does a detailed survey of the area where he wants to live, in which he quantifies, normalizes, and maps the desirable features of houses to values on a scale of  to  so the data can be assembled into a table. If Charlie noted  features, each row contains  space-separated values followed by the house price in dollars per square foot (making for a total of  columns). If Charlie makes observations about  houses, his observation table has  rows. This means that the table has a total of  entries.

Unfortunately, he was only able to get the price per square foot for certain houses and thus needs your help estimating the prices of the rest! Given the feature and pricing data for a set of houses, help Charlie estimate the price per square foot of the houses for which he has compiled feature data but no pricing.

Important Observation: The prices per square foot form an approximately linear function for the features quantified in Charlie's table. For the purposes of prediction, you need to figure out this linear function.

Recommended Technique: Use a regression-based technique. At this point, you are not expected to account for bias and variance trade-offs.

Input Format

The first line contains  space-separated integers,  (the number of observed features) and  (the number of rows/houses for which Charlie has noted both the features and price per square foot).
The  subsequent lines each contain  space-separated floating-point numbers describing a row in the table; the first  elements are the noted features for a house, and the very last element is its price per square foot.

The next line (following the table) contains a single integer, , denoting the number of houses for for which Charlie noted features but does not know the price per square foot.
The  subsequent lines each contain  space-separated floating-point numbers describing the features of a house for which pricing is not known.


There are multiple ways to approach this problem that account for bias, variance, various subjective factors, and "noise". We take a realistic approach to scoring and permit up to a  swing of our expected answer.
