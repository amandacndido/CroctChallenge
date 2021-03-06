<p align="center"> CroctChallenge

>Status: Finalized

# Create user's stories based in a sign in and sign up scenarios. 
  This repository was created in order to submit to Croct my abilities and to fulfill the challenge proposed. My task is to describe all possible scenarios involving the sign-in/sign-up pages, create the user's stories and write how the interface should behave.
  
## Sign In
 
<br /> 

>**Scenario: Changing to a new password**
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
> Then I should see a notification saying _"Your password has been successfully changed! "_
  
<br />
  
>**Scenario: Inserting a wrong password** 
>
> Given that I am a registered user in the *Sign in* page
>
> When I enter a wrong password
>
> And I click the *Sign in* button
>
> Then I should see a notification saying _"Your password is incorrect. Forget your password?"_
  
<br />  
  
>**Scenario: Searching for the user's account in order to recorver the password** 
>
> Given that I am a registered user in the *Sign in* page
>
> When I click the *Forgot password?* button
>
> Then I should see a section saying _"Find your account: Insert your email address"_

<br /> 
  
>**Scenario: Searching for the user's account with valid information** 
>
> Given that I click the *Forgot password?* button
>
> When I see a section saying  _"Find your account: Insert your email: "_ 
>
> And I insert valid information
>
> And I click *Next*
>
> Then I should see a notification saying _"A new password has been sent to your email"_
  
<br />  
  
>**Scenario: Searching for the user's account with invalid information** 
>
> Given that I click the *Forgot password?* button
>
> When I see the _"Find your account: Insert your email:"_ section
>
> And I insert invalid information
>
> And I click *Next*
>
> Then I should see a notification saying _"Email not found. Check your informations and insert it again"_

<br />  
  
>**Scenario: Changing to a new password with two-step verification activated** 
>
> Given that the *two-step verification* option in my account is activated
>
> And I click the button *"Forgot password?"*
>
> When I see a section saying: _"Find your account: Insert your email:"_
>
> And I insert a valid email
>
> And I click *Next*
>
> Then I should see a notification saying _"Insert the code sent to your email"_
  
<br />  
 
>**Scenario: Receving a code from Croct in two-step verification** 
>
> Given that I see a section saying: _"Find your account: Insert your email:"_
>
> When I insert a valid email
>
> And click *Next*
>
> Then I should receive a code from Croct in my inbox

 <br />  
  
>**Scenario: Inserting a wrong code in the two-step verification** 
>
> Given that I see the notification saying _"Insert the code sent to your email"_
>
> When I insert the wrong verification code
>
> And I click to "Verify code"
>
> Then I should see a notification saying _"The  inserted code is incorrect. `Send a new code?`"_
  
<br />  
  
>**Scenario: Inserting the right code in the two-step verification** 
>
> Given that I see the notification saying _"Insert the code sent to your email"_
>
> When I insert the right verification code
>
> And I click to "Verify code"
>
> Then I should see a notification saying _"Code verified. Insert your new password: "_


  
<br />  
  
## Sign up

<br />  
  
>**Scenario: Accessing Terms of service** 
>
> Given that I am in the Sign up screen 
>
> And I insert all necessary information
>
> When I click the "Terms of services" section 
>
> Then I should see a popup notification that contains all Terms of service
  
<br />
  
>**Scenario: Accessing Privacy policy** 
>
> Given that I am in the Sign up screen 
>
> And I insert all necessary information
>
> When I click the _"Privacy policy"_ section 
>
> Then I should see a popup notification that contains all Privacy policy details
  
<br />  
  
>**Scenario: Succesfuly creating an account**  
>
> Given that I insert valid information in the Sign up screen
>
> And I select the "I agree to the Terms of Service and Privacy Policy" checkbox 
>
> And I click the "Sign Up" button
>
> Then I should see a notification saying "Your account has been created!"
  
<br /> 
  
>**Scenario: Confirm email request** 
>
> Given that I successfully created my new account
>
> When I access my profile
>
> Then I should see a popup notification with a button saying "Confirm your email" 

<br />  
  
>**Scenario: Receive email confirmation** 
>
> Given that I click the "Confirm your email" button
>
> When I access my inbox
>
> Then I should see a "Confirm my email address" button in an email sent by Croct
  
<br />
  
>**Scenario: successfully confirming an email**  
>
> Given that I click the "Confirm my email address" button in my inbox
>
> When I am redirectioned to a new Croct screen saying "Your email has been confirmed. `Go back to your account` "
>
> And I click the `Go back to your account` button
>
> Then I should be sent to my account 
 
<br />
  
>**Scenario: Trying to sign in with a non registered account** 
>
> Given that I am not registered 
>
> And I try to Sign in
>
> Then I should see a notification saying "User not registered. Create a new account?"

<br />
  
>**Scenario: Acessing the Sign up screen trough the Sign in screen** 
>
> Given that I am in the Sign in screen
>
> When I click in the button saying "Sign up" 
>
> Then I should be redirectioned to the Sign up screen

<br />
  
>**Scenario: Acessing the Sign in screen trough the Sign up screen** 
>
> Given that I am in the Sign up screen
>
> When I click in the button saying "Sign in" 
>
> Then I should be redirectioned to the Sign in screen

<br />

>**Scenario: Not selecting the Terms of Service and Privacy Policy checkbox** 
>
> Given that I insert all needed information in the Sign up screen
>
> And I don't select the "I agree to the Terms of Service and Privacy Policy" checkbox 
>
> When I click the "Sign Up" button
>
> Then I should see a notification saying "Accept the Terms of Service and Privacy Policy before continue"

 <br /> 
  
>**Scenario: Trying to sign up with a registered email** 
>
> Given that I insert data previously registered
>
> And I select the "I agree to the Terms of Service and Privacy Policy" checkbox 
>
> And I click to "Sign up"
>
> Then I should see a notification saying "Registered user. Do you want to `access you account?`" 
 
 <br /> 
  
>**Scenario: Acessing the Sign in screen through the "Registered user " notification**  
>
> Given that I see the notification saying "Registered user. Do you want to `access you account?` "
> 
> And I click the `access you account?` option
>
> Then I should be redirectioned to the Sign in screen


