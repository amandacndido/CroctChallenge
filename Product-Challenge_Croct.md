<p align="center"> CroctChallenge

>Status: Developing

# Create user's stories based in a sign in and sign up scenarios. 
  This repository was created in order to submit to Croct my abilities and to fulfill the challenge proposed. My task is to describe all possible scenarios involving the sign-in/sign-up pages, create the user's stories and write how the interface should behave.
  
## Sign In
  Forgot password User's stories:
   

**Scenario: Changing to a new password**
>
> Given that I am a registered user 
>
> And click the *Forgot password?* button
>
> When I enter a new password `NewPassword1*` 
> 
> And I enter the same password `NewPassword1*` in the *Confirm Password* section 
>
> And I click to *Save*
> 
> Then I should see a notification saying _"Your password has been changed successfully! "_
  
  
  
**Scenario: Inserting a wrong password**
> Given that I am in the *sign in* page
>
> And I am registered user
>
> When I enter a wrong password
>
> And I click the *Sign in* button
>
> Then I should see a notification saying _"Your password is incorrect. Forget your password?"_
  
  
  
**Scenario: Searching for the user's account in order to recorver the password
> Given that I click the *Forgot password?* button
>
> Then I should see a section saying _"Find your account: Insert your email or username"_

  
  
**Scenario: Searching for the user's account with valid information
> Given that I click the *Forgot password?* button
>
> And I see the _"Find your account: Insert your email or username"_ section
>
> And I insert valid information
>
> Then I should see a notification saying "A new password has been sent to your email"
  
  
  
**Scenario: Searching for the user's account with invalid information
> Given that I click the *Forgot password?* button
>
> And I see the _"Find your account: Insert your email or username" section
>
> And I insert not valid information
>
> Then I should see a notification saying "Email or username not found. Check your informations and insert it again"

  
  
**Scenario: Changing to a new password with two-step verification activated (e-mail)
> Given that I activated the *two-step verification* option in my account
>
> And I click the button "Forgot password?" 
>
> When I see a section saying: "Insert your phone number or email in order to receive a code"
>
> And I insert a valid email
>
> Then I should see a notification saying "Insert the code sent to your email" 
  
  
  
**Scenario: Changing to a new password with two-step verification activated (phone number)
> Given that the *two-step verification* option in my account is activated
>
> And I click the "Forgot password?" button
>
> When I see a section saying: "Insert your phone number or email in order to receive a code"
>
> And I insert a valid phone number
>
> Then I should see a notification saying "Insert the code sent to your phone" 
  
 
**Scenario: Inserting a wrong code in the two-step verification (email)
> Given that the *two-step verification* option in my account is activated
>
> And I click the "Forgot password?" button
>
> When I see a section saying: "Insert your phone number or email in order to receive a code"
>
> And I insert a valid phone email
>
> And I see a notification saying "Insert the code sent to your email" 
>
> When I insert the wrong verification code
>
> Then I should see a notification saying "The  inserted code is incorrect. Send a new code?"
  
  
**Scenario: Inserting a wrong code in the two-step verification (phone number)
> Given that the *two-step verification* option in my account is activated
>
> And I click the "Forgot password?" button
>
> When I see a section saying: "Insert your phone number or email in order to receive a code"
>
> And I insert a valid phone number
>
> And I see a notification saying "Insert the code sent to your phone number" 
>
> When I insert the wrong verification code
>
> Then I should see a notification saying "The  inserted code is incorrect. Send a new code?"
  

**Scenario: Insertin the right code in the two-step verification
> Given that the *two-step verification* option in my account is activated
>
> And I click the "Forgot password?" button
>
> When I see a section saying: "Insert your phone number or email in order to receive a code"
>
> And I insert a valid phone number/ email
>
> And I see a notification saying "Insert the code sent to your phone" 
>
> When I insert the rigt verification code
>
> Then I should see a section saying "Insert your new password"
  
  
## Sign up

  
**Scenario: Accessing Terms of service
> Given that I am in the Sign up screen 
>
> And I insert all necessary information
>
> And I click the "Terms of services" section on the sign up screen
>
> Then I should see a popup notification that contains all Terms of service
  

**Scenario: Accessing Privacy policy
> Given that I want to acces the Privacy policy 
>
> And I click the "Privacy policy" section on the sign up screen
>
> Then I should be redirectioned to a new page that contain all Privacy policy details
  
  
  
**Scenario: Succesfuly creating an account
> Given that I insert valid information in the sign up screen
>
> And I select the "I agree to the Terms of Service and Privacy Policy" checkbox 
>
> And I click the "Sign Up" button
>
> Then I should see a notification saying "Your account has been created!"
  
  
 **Scenario: Confirm email
> Given that I sucessfully create my new account
>
> When I access my profile
>
> Then I should see a "Confirm your email" notification
  
  
**Scenario: Trying to sign in with a non registered account
> Given that I am not registered 
>
> And I try to sign in
>
> Then I should see a notification saying "User not registered. Create a new account?"


**Scenario: Acessing the sign up screen trough the sign in screen
> Given that I am in the sign in screen
>
> When I click in the button "Sign up" 
>
> Then i should be redirectioned to the sign up screen

  
**Scenario: Acessing the sign in screen trough the sign ip screen
> Given that I am in the sign up screen
>
> When I click in the button "Sign in" 
>
> Then i should be redirectioned to the sign in screen



**Scenario: Not selecting the Terms of Service and Privacy Policy checkbox
> Given that I insert all needed information in the Sign up screen
>
> And I don't select the "I agree to the Terms of Service and Privacy Policy" checkbox 
>
> When I click the "Sign Up" button
>
> Then I should see a notification saying "Accept the Terms of Service and Privacy Policy before continue"
  
  
**Scenario: Trying to sign up with a registered email
> Given that I insert data previously registered
>
> And I select the "I agree to the Terms of Service and Privacy Policy" checkbox 
>
> And I click to "Sign up"
>
> When I see a notification saying "Registered user. Do you want to `access you account?` "
> 
> And I click the `access you account?` option
>
> Then I should be redirectioned to the Sign in screen


