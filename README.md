# Ticket Cancellation Prediction Using XGBoost

This project aims to predict whether a travel booking will be canceled or not based on booking data from the Mr. Bilit website. Cancellations are costly for the company, as it has to pay penalties for each canceled booking. Therefore, identifying bookings with a high likelihood of cancellation can greatly assist in risk management. 

The algorithm used for this prediction is **XGBoost**, a gradient boosting method known for its efficiency in classification tasks.


## Dataset

The dataset used in this project is sourced from travel booking data provided by Mr. Bilit website. The dataset includes information from various users and their travel bookings, including trip details, personal information, and ticket attributes.

**Note:** The dataset is proprietary, and thus, its publication is not permitted.

### Dataset Description

The dataset consists of travel booking records and includes the following columns:

| Column                  | Description                                        |
|-------------------------|----------------------------------------------------|
| `Created`               | Timestamp when the booking was made               |
| `CancelTime`            | Timestamp when the ticket was canceled            |
| `DepartureTime`         | Scheduled departure time of the trip              |
| `BillID`                | Purchase ID                                       |
| `TicketID`              | Ticket ID                                         |
| `ReserveStatus`         | Customer payment status                           |
| `UserID`                | Unique user ID                                    |
| `Male`                  | Gender of the passenger                           |
| `Price`                 | Price of the ticket without discounts             |
| `CouponDiscount`        | Discount applied to the ticket                    |
| `From`                  | Departure location                                |
| `To`                    | Destination location                              |
| `Domestic`              | Whether the trip is domestic or international     |
| `VehicleType`           | Type of vehicle used for the trip                 |
| `VehicleClass`          | Whether the vehicle is first-class or not         |
| `Vehicle`               | Specific vehicle used                             |
| `HashPassportNumber_p`  | Hashed passport number                            |
| `HashEmail`             | Hashed email address                              |
| `BuyerMobile`           | Hashed mobile number                              |
| `NationalCode`          | Hashed national ID                                |
| `TripReason`            | Reason for the trip                               |
| `Cancel`                | Whether the ticket was canceled (target variable) |

### Dataset Location

- **Data/**: This folder will contain the dataset files.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**

## Project Structure

The main folders and files in the project are structured as follows:

```plaintext
Travel-Cancellation-Prediction/
├── Data/
│   └── [dataset files will be here]
├── Notebook/
│   └── [your Jupyter notebooks will be here]
└── README.md
```

## Feature Engineering and Data Preprocessing

- **Identifying and creating new features** 
- **Handling missing values** 
- **Encoding categorical variables** 
- **Scaling numerical features** 
- **Splitting the dataset**


## Model Training
The model is trained using the **XGBoost** algorithm. The model predicts the likelihood of a ticket being canceled based on user and booking-related features.

## Model Performance

The model achieved the following F1 scores:
- **Training Set:** 0.9620
- **Test Set:** 0.9410

## Requirements
To run this project, you'll need the following Python libraries:
- `pandas`
- `scikit-learn`
- `xgboost`
