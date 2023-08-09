# Andes Paradise

## Table of Contents
- [Overview](#overview)
- [Built With](#built-with)
- [Features](#features)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

## Overview
<!-- ![alt text](public/pinoen-dark.svg) -->
<img src='public/pinoen-dark.svg' width='120px'>

- "Andes Paradise" is a small boutique hotel with initially 8 luxurious wooden cabins.
- The owners needed a custom-built application to manage everything about the hotel: bookings, cabins and guests.
- This is an internal application used inside the hotel to check in guests as they arrive.
- They also needed the API.
- Later they will probably want a customer-facing website as well, where customers will be able to book stays, using the same API
- It was built with React using Vite.
- You can try it out at [Vercel - Andes Paradise](https://andes-paradise-smdla.vercel.app). Email: pinoen@example.com - password: admin

### Built With
- Routing: React Router
- Styling: styled components
- Remote State Management: React Query
- UI State Management: Context API
- Form Management: React Hook Form
- Back-end database and API: Supabase
- Other tools:
  - React Icon
  - React hot toast
  - Recharts
  - date-fns
  - React Error Boundary

## Features
- Users of the app are hotel employees. They need to be logged into the application to perform tasks.
![Login](public/pages/login.png)

- New users can only be signed up inside the applications (to guarantee that only actual hotel employees can get accounts).
![Signup](public/pages/signup.png)

- Users should be able to upload an avatar, and change their name and password.
![Account settings](public/pages/account.png)

- App needs a table view with all cabins, showing the cabin photo, name, capacity, price, and current discount.
- Users should be able to update or delete a cabin, and to create new cabins (including uploading a photo).
![Cabins](public/pages/cabins.png)

- App needs a table view with all bookings, showing arrival and departure dates, status, and paid amount, as well as cabin and guest data.
- The booking status can be “unconfirmed” (booked but not yet checked in), “checked in”, or “checked out”. The table should be filterable by this important status.
![Bookings](public/pages/bookings.png)

- Other booking data includes: number of guests, number of nights, guest observations, whether they booked breakfast, breakfast price.
- Users should be able to delete, check in, or check out a booking as the guest arrives (no editing necessary for now).
- Bookings may not have been paid yet on guest arrival. Therefore, on check in, users need to accept payment (outside the app), and then confirm that payment has been received (inside the app).
- On check in, the guest should have the ability to add breakfast for the entire stay, if they hadn’t already.
- Guest data should contain: full name, email, national ID, nationality, and a country flag for easy identification.
![Booking details](public/pages/details.png)

- The initial app screen should be a dashboard, to display important information for the last 7, 30, or 90 days:
  - A list of guests checking in and out on the current day. Users should be able to perform these tasks from here
  - Statistics on recent bookings, sales, check ins, and occupancy rate
  - A chart showing all daily hotel sales, showing both “total” sales and “extras” sales (only breakfast at the moment)
  - A chart showing statistics on stay durations, as this is an important metric for the hotel
  ![Dashboard](public/pages/dashboard.png)  

- Users should be able to define a few application-wide settings: breakfast price, min and max nights/booking, max guests/booking.
![Login](public/pages/settings.png)

- App needs a dark mode.
![Login](public/pages/dark-mode.png)

### From those requirements, the app needs these pages:
  1. Dashboard
  2. Booking
  3. Cabins
  4. Booking checkin
  5. App settings
  6. User sign up
  7. Login
  8. Account settings

## Acknowledgements
This project is part of The Ultimate React Course 2023: React, Redux & More by [Jonas Schmedtmann](http://jonas.io/).