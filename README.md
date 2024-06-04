# Smart-Weather-Station-ESP32

The code checks if the temperature or humidity are outside the normal ranges and marks the conditions as severe.
If severe conditions are detected, it sends an alert message along with the weather data to the Flask server.
Flask Server:

Receives the weather data and alert messages from the ESP32.
If it receives an alert message, it sends an alert email using SMTP.
Configuration for sending emails:
SMTP_SERVER: The address of the SMTP server (e.g., smtp.gmail.com for Gmail).
SMTP_PORT: The port for the SMTP server (usually 587 for TLS).
SMTP_USERNAME: Your email address.
SMTP_PASSWORD: Your email password or the generated application password.
EMAIL_FROM: The email address from which the message is sent.
EMAIL_TO: The list of recipients who will receive the weather alerts.
