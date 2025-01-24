# Automated Stock Trading

A Django-based web application for managing stock trading activities, where users can view, trade, and manage stocks. Admins can manage users and stocks through a dedicated admin interface.

## Features

### For Guests:
- **Homepage**: Introduction to the platform.
- **Login**: Access your account if registered.
- **Signup**: Register a new account.
- **Forget Password**: Reset your password.

### For Registered Users:
- **Logout**: Log out from your account.
- **User Dashboard**: View user-specific information.
- **Profile Page**: View and edit your profile.
- **Stocks Page**: Browse available stocks.
- **Stock View**: View detailed stock information.
- **My Stocks**: View and manage owned stocks.
- **Place Bid on Stock**: Bid on available stocks.
- **Sell Stock**: Sell stocks you own.

### For Admin Users:
- **Admin Dashboard**: Manage and view users and stocks.
- **Manage Users**: View, edit, and delete user profiles.
- **Manage Stocks**: Add, edit, or delete stocks.
- **View User Stocks**: View stocks owned by users.

### Common Pages:
- **Terms and Conditions**: Platform terms and policies.
- **Privacy Policy**: User privacy policy.

## Installation

Follow the steps below to install and run the project locally.

### Prerequisites
- Python 3.x
- Django 3.2
- PostgreSQL (or other database options)

### Steps

1. **Clone the repository**:
   ```bash
   git clone https:https://github.com/anurag8773/Stock-Trading-System/
   ```

2. **Navigate to the project directory**:
   ```bash
   cd Stock-Trading-System
   ```

3. **Set up a virtual environment**:
   ```bash
   python3 -m venv venv
   ```

4. **Activate the virtual environment**:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

5. **Install required dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

6. **Set up the database**:
   Run the following command to apply migrations:
   ```bash
   python manage.py migrate
   ```

7. **Create a superuser**:
   Run this command to create an admin account:
   ```bash
   python manage.py createsuperuser
   ```

8. **Run the development server**:
   ```bash
   python manage.py runserver
   ```

9. **Access the application**:
   Open your browser and go to `http://127.0.0.1:8000/` to access the application.

## URL Configuration

### For Guests:
- `/`: Homepage
- `/login`: Login page
- `/signup`: Signup page
- `/forget_password`: Password reset page

### For Registered Users:
- `/logout`: Log out of the user account
- `/user_page`: User dashboard
- `/profile`: User profile page
- `/edituserprofile`: Edit user profile
- `/stock`: Browse available stocks
- `/stockView/<int:id>`: View detailed stock information
- `/mystocks`: View owned stocks
- `/bidToStock/<int:id1>/<int:id2>`: Place a bid on a stock
- `/sold_stock/<int:id1>/<int:id2>`: Sell a stock

### For Admin Users:
- `/admin`: Admin dashboard
- `/adminlogin`: Admin login
- `/adminhome`: Admin homepage
- `/adminalluser`: View all users
- `/adminprofile`: Admin profile page
- `/adminlogout`: Admin logout
- `/view_user/<int:id>`: View a specific user
- `/adminEditUserProfile/<int:id>`: Edit a user profile
- `/deleteuser/<int:id>`: Delete a user
- `/admin_stock`: View all stocks
- `/admin_stockView/<int:id>`: View a specific stock
- `/deletestock/<int:id>`: Delete a stock
- `/admin_update_stock/<int:id>`: Update stock details
- `/admin_add_stock`: Add a new stock
- `/admin_view_user_stock/<int:id>`: View a user's stocks

### Common Pages:
- `/terms_and_condition`: Terms and conditions page
- `/privacy_policy`: Privacy policy page

## Dependencies

- **Django**: The web framework used for this project.
- **PostgreSQL** (or other database engines supported by Django): Database for storing user and stock information.
- **Django REST Framework**: For building APIs if necessary.

Install the required dependencies using:

```bash
pip install -r requirements.txt
```

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -am 'Add new feature'`
4. Push to your branch: `git push origin feature-name`
5. Submit a pull request.

## Acknowledgments

- **Django**: For providing a robust web framework.
- **PostgreSQL**: For serving as the database backend.
```
