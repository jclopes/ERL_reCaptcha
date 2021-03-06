# Project:
Erlang reCaptcha API


# Description:
This erlang module implements some functions that simplify the use of reCapture service.


# Manual:
  - Request Challenge: display_html(PublicKey, UseSSL, Error)
    - PublicKey: Your reCaptcha public_key.
    - UseSSL: Set to 'true' if you want to use a SSL connection.
    - Error: An error message to display.
  - Response Validation: submit(PrivateKey, RemoteIp, Challenge, Response)
    - PrivateKey: Your reCAPTCHA private key.
    - RemoteIp: The user's IP address.
    - Challenge: The value of recaptcha_challenge_field from the form.
    - Response: The value of recaptcha_response_field from the form.


# Acknowledgement:
  - The reCAPTCHA service is an amazing tool that help us all keep the internet a better place. [link](http://recaptcha.net)
  - The implementation was inspired by the python recaptcha-client. [link](http://pypi.python.org/pypi/recaptcha-client)
  - This project uses the code from Buddy Moore erlang driver. [link](http://code.google.com/p/recaptcha-erlang)
