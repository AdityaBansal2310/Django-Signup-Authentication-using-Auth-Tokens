# Django-Signup-Authentication-using-Auth-Tokens


# Using Postman for Authentication Requests

## Register a New User

1. Open Postman and create a new request.
2. Set the request method to `POST`.
3. Enter the URL: `http://localhost:8000/api/register/`.
4. Add a header:
   - **Key:** `Content-Type`
   - **Value:** `application/json`
5. In the Body tab, select raw and choose JSON.
6. Enter the following JSON data:
   ```json
   {
       "username": "testuser",
       "password": "testpassword",
       "email": "test@example.com"
   }
7. Click send to send the request.



## Login with the Registered User

1. Create a new request in Postman.
2. Set the request method to POST.
3. Enter the URL: `http://localhost:8000/api/login/`.
4. Add a header:
   - Key: `Content-Type`
   - Value: `application/json`
5. In the Body tab, select raw and choose JSON.
6. Enter the following JSON data:
   ```json
   {
       "username": "testuser",
       "password": "testpassword"
   }
7. Click Send to make the request.




## Logout Using the Authentication Token

1. Create a new request in Postman.
2. Set the request method to POST.
3. Enter the URL: `http://localhost:8000/api/logout/` (assuming correct logout endpoint).
4. Add a header:
   - Key: `Authorization`
   - Value: `Token YOUR_AUTH_TOKEN` (replace `YOUR_AUTH_TOKEN` with the actual token obtained during login).
5. Click "Send" to make the request.


### Make sure to replace placeholders like `YOUR_AUTH_TOKEN` with actual values.
