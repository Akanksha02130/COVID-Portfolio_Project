
# COVID-19 Data Analysis Project

## Project Description
This project involves the analysis of COVID-19 data, specifically focusing on COVID-19 deaths, cases, vaccinations, and population statistics across different locations and continents. The goal is to gain insights into the impact of the pandemic, including mortality rates, vaccination coverage, and infection rates relative to the population. The data is sourced from the "PortfolioProject" database.

## Problem Statement
The project aims to address several key questions related to the COVID-19 pandemic, including:
- What is the likelihood of dying if someone contracts COVID-19 in a specific country or location (e.g., states)?
- What percentage of a population has contracted COVID-19 in various locations?
- Which countries have the highest infection rates relative to their population?
- What continents have the highest and lowest death counts per population?
- What are the global COVID-19 statistics, including total cases, total deaths, and the death percentage?

## Solution
The project employs a series of SQL queries to analyze and extract meaningful insights from the COVID-19 data. It follows these steps:

1. Selects relevant columns from the "CovidDeaths" table, filtering out records with null continents, and orders the data by location and date.
2. Alters the data type of the "total_cases" column in the "CovidDeaths" table to float.
3. Calculates the death percentage based on total cases and total deaths for locations containing the term "states" in their names.
4. Analyzes the percentage of a population that contracted COVID-19 by dividing total cases by the population for each location.
5. Identifies countries with the highest infection rates compared to their population.
6. Identifies the country with the highest death count per population.
7. Breaks down the data by continent, showing continents with the highest and lowest death counts per population.
8. Computes global COVID-19 statistics, including total cases, total deaths, and the death percentage.
9. Alters the data type of the "new_vaccinations" column in the "CovidVaccinations" table to float.
10. Joins the "CovidDeaths" and "CovidVaccinations" tables to examine the relationship between population, vaccinations, and COVID-19 cases over time.
11. Utilizes a common table expression (CTE) to simplify the query structure and maintain the rolling sum of vaccinated people over time.
12. Creates a temporary table to store data for later analysis.
13. Creates a view named "PercentPopulationVaccinated" to store data for visualization purposes.

## Conclusion
This project provides valuable insights into the COVID-19 pandemic's impact, including death rates, infection rates relative to the population, and the progress of vaccinations. It enables the identification of countries and continents with the highest and lowest pandemic-related statistics. The project also prepares data for potential visualization and further analysis.
