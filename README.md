In this exercise, you will be automating login process with email address and OTP.

### Prerequisites

- Install IntelliJ IDEA Community IDE  Version 2018.3.6.
- Install OpenJDK 11 and complete the configuration.
- Install a Browser Driver(Chrome Driver).
- Setup a Selenium project with the name `OtpLoginTest`.

You can refer to this [Reading Material](https://learning.ccbp.in/qa-automation-testing/course?c_id=cf952b35-27ab-4b1e-a6de-44227f22806c&s_id=f5c19277-3889-4e63-b631-c06c088d612c&t_id=c82e95ce-1faf-4acb-9021-476a9359da79#31-install-ide) to complete the above prerequisites.

### Steps to Automate

- Create a driver instance using WebDriver interface.
- Navigate to the url `https://practice.expandtesting.com/otp-login`
- Enter the email address and print "Email address entered" - _use id locator_.
  
  - Email Address: `practice@expandtesting.com`
- Click on the "Send OTP Code" - _use className locator with value `mb-3`_.(Use submit() method).
- Verify if the current page title matches the expected page title(Test Automation Practice: Working with OTP Verification).
- If both expected and current page titles are same

  - Print "OTP sent successfully".
  - Print current page title in a new line.
- Else print "Enter valid email".
- Enter the OTP and print "OTP entered"- _use id locator_.
  
  - OTP: `214365`
- Click on the "Verify OTP Code" button - _use id locator_.(Use submit() method).
- Wait for a maximum of 10 seconds for the web page to be redirected.
- Verify if the current URL matches the expected URL (https://practice.expandtesting.com/secure).
- If both expected and current URLs are same

    - Print "Logged in successfully"
    - Print current page title in a new line.
- Else print "Log in failed!"
- Close the browser window.

**Set up the project and practice this exercise in your local IDE(IntelliJ). Click on the `OPEN IDE` button to refer to the folder structure.**