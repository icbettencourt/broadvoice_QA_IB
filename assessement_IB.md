# What questions would you ask in order to clarify requirements?

What happens if:

**1.**	the first and last names have some special characters or spaces? e.g. Maria João

**2.**	the email, first name and last name have more or less than the defined characters?

**3.**	the email doesn’t follow the correct format? e.g.: name@example.ex

**4.**	the email is already registered?

**5.**	the user doesn’t want their credentials on the home page after login?

**6.**	the user tries to register without filling one of the fields?

**7.**	the user doesn’t receive the email with a temporary password?

**8.**	the new password needs to have a number of characters? Needs to have at least a capital letter, one digit or character?

**9.**	the user creation process takes more than 3 seconds?  


# Specify 5 test cases to test this requirement

Check if:

**1.**	the variables have the correct length or accept special characters or spaces.

**2.**	an email without @example.ex is accepted or rejected

**3.**	the email is already registered in database

**4.**	clicking the “save” button stores the user in database

**5.**	the user receives the email with the temporary password

