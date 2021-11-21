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
> And I am registerd user
>
> When I enter a wrong user password
>
> And I click the *Sign in* button
>
> Then I should see a notification saying _"Your password is incorrect. Forget your password?"_
  
  
  
**Scenario: Searching for the user's account
> Given that I click the *Forgot password?* button
>
> Then I should see a section saying _"Find your account: Insert your e-mail or username"_

  
  
**Scenario: Searching for the user's account with valid information
> Given that I click the *Forgot password?* button
>
> And I see the _"Find your account: Insert your e-mail or username"_ section
>
> And I insert valid information
>
> Then I should see a notification saying _"A new password has been sent to your e-mail"
  
  
  
**Scenario: Searching for the user's account with invalid information
> Given that I click the *Forgot password?* button
>
> And I see the _"Find your account: Insert your e-mail or username"_ section
>
> And I insert not valid information
>
> Then I should see a notification saying _"E-mail not found. Check your informations and insert again"

  
  
**Scenario: Changing to a new password with two-step verification activated
> Given that I activated the *two-step verification* option in my account
>
> And I click the "Forgot password?" button
>
> And I insert a valid e-mail
>
> Then I should see a "Insert the code sent to your e-mail" notification before change the password
  
**Scenario: Think about a new one

## Sign up
  Terms of service User's stories
  
**Scenario: 

