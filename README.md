# Netflix-SQL
Netflix Movies and TV Shows Data Analysis using SQL
![image](https://github.com/user-attachments/assets/27cda6f0-9f98-4066-bd8d-69705b0b07dc)

# Overview
This project involves a comprehensive analysis of Netflix's movies and TV shows data using SQL. The goal is to extract valuable insights and answer various business questions based on the dataset. The following README provides a detailed account of the project's objectives, business problems, solutions, findings, and conclusions.

# Objectives
- Analyze the distribution of content types (Movies vs TV shows).
- Identify the most common ratings for movies and TV shows.
- List and analyze content based on release years, countries, and durations.
- Explore and categorize content based on specific criteria and keywords.

# Dataset
https://www.kaggle.com/datasets/shivamb/netflix-shows?resource=download

# Schema
DROP TABLE IF EXISTS netflix;
CREATE TABLE netflix
(
    show_id      VARCHAR(5),
    type         VARCHAR(10),
    title        VARCHAR(250),
    director     VARCHAR(550),
    casts        VARCHAR(1050),
    country      VARCHAR(550),
    date_added   VARCHAR(55),
    release_year INT,
    rating       VARCHAR(15),
    duration     VARCHAR(15),
    listed_in    VARCHAR(250),
    description  VARCHAR(550)
);

# Business Problems and Solutions

# 1. Count the Number of Movies vs TV Shows
select type , count(*)
from netflix 
group by type;

# 2. Find the Most Common Rating for Movies and TV Shows









