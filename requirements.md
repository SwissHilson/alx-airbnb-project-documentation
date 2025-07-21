# Airbnb Clone - Backend Requirements

## User Authentication

### Endpoints:
- POST /api/v1/register
- POST /api/v1/login

### Inputs:
- email
- password

### Outputs:
- JWT token
- success or error messages

### Validations:
- Unique email
- Strong password rules

---

## Property Management

### Endpoints:
- POST /api/v1/properties
- GET /api/v1/properties
- PUT /api/v1/properties/{id}
- DELETE /api/v1/properties/{id}

### Inputs:
- name
- description
- price
- amenities
- photos

### Outputs:
- Property details JSON

---

## Booking System

### Endpoints:
- POST /api/v1/bookings
- GET /api/v1/bookings
- DELETE /api/v1/bookings/{id}

### Inputs:
- property_id
- user_id
- start_date
- end_date

### Outputs:
- Booking confirmation
- Error handling

### Rules:
- Check for date conflicts
- Only logged-in users can book

