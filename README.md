# Hotel Recommendation System

## Table of Contents
1. [Background](#background)
2. [Problem Statement](#problem-statement)
3. [Approach](#approach)
4. [Dataset](#dataset)
5. [Data Preprocessing and Cleaning](#data-preprocessing-and-cleaning)
6. [Results](#results)
7. [Demo](#demo)
8. [Future Work](#future-work)
9. [Contributors](#contributors)
10. [License](#license)

## Background

In the ever-evolving travel and hospitality industry, it is crucial to provide users with accurate and personalized hotel recommendations. This project aims to address the difficulty users face when trying to find the best hotels suited to their needs and preferences during vacations.

This project is part of the **DSCO Final 2023** competition, where we developed a **Hotel Recommendation System** to assist users in selecting hotels based on their preferences, using machine learning techniques.

## Problem Statement

With the vast number of hotels available worldwide, travelers often struggle to find the best options suited to their preferences, such as room types, amenities, location, and price range. The challenge is to predict the most suitable hotels for users by leveraging historical data and hotel features.

## Goal

Our goal is to build a **hotel recommendation system** that can:
- Suggest the best hotels based on various attributes like room types, amenities, location, and price ranges.
- Offer personalized hotel suggestions to users based on their preferences.

## Approach

We use a **content-based filtering approach** for the recommendation system. Unlike collaborative filtering, which relies on user-item interactions, content-based filtering uses information about the hotels (e.g., room types, amenities, price, etc.) to make recommendations. Here’s the step-by-step approach:

1. **Data Collection**: We collect data from multiple sources including hotel attributes, pricing, amenities, and location information.
2. **Data Preprocessing**: The raw data is cleaned by handling missing values, encoding categorical variables, and normalizing numerical values.
3. **Feature Extraction**: Key features such as room amenities, star ratings, property type, and location are extracted to build a feature matrix.
4. **Similarity Calculation**: Using techniques like **TF-IDF** (Term Frequency-Inverse Document Frequency), we calculate the similarity between hotels based on their features.
5. **Recommendation Generation**: Once similarities are computed, the system recommends hotels by ranking them based on similarity to a user’s preferences.

### Key Techniques Used:
- **Content-based Filtering**: We recommend hotels based on their features such as room type, amenities, price, etc.
- **TF-IDF Vectorization**: Used for processing and analyzing textual data such as room descriptions and amenities.

## Dataset

The dataset used in this project includes:
- **Hotel Details**: Information about the hotel such as hotel name, city, country, and star rating.
- **Room Price Data**: Pricing and availability details for each room type.
- **Hotel Amenities**: Features such as Wi-Fi, air conditioning, in-room safe, etc.

**[Hotel Recommendation Dataset (Kaggle)](https://www.kaggle.com/datasets/keshavramaiah/hotel-recommendation)**

## Data Preprocessing and Cleaning

Several steps were taken to clean and prepare the data:
- Missing values were handled by imputing or dropping columns.
- Certain irrelevant columns were removed (e.g., `zipcode`, `latitude`, `longitude`).
- Categorical columns like room types and amenities were encoded for machine learning compatibility.

## Results

The recommendation system successfully provides hotel suggestions based on key features. The model performs well, with a **precision@5** of **1.0** during evaluation, meaning that all top 5 recommendations were relevant. The recommendations are tailored to users’ preferences, ensuring a personalized experience.

## Demo

https://github.com/user-attachments/assets/230f4fe0-798e-40b8-852c-be256fafac2f

## Future Work

- **Enhanced Feature Engineering:** Explore additional features like hotel reviews, star ratings, and geographical data to further refine the model.
- **Deep Learning Models:** Incorporating deep learning methods for more complex feature extraction and recommendation generation.
- **Real-Time Recommendations:** Implement a recommendation system that offers real-time suggestions based on changing availability and prices.

## Contributors

- **Steve Marcello Liem**
- **Davin Edbert Santoso Halim**
- **Brandon Ritchie Yang**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
