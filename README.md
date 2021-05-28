# Python-Password-Manager
Objective: To develop a custom password manager using Python   
Domain:  Security
Steps to perform:
   
    class BasePasswordManager
      members
        old_passwords: is a list that holds all of the user's past passwords.
        The last item of the list is the user's current password.

      methods
        get_password method that returns the current password as a string.
        is_correct method that receives a string and returns a boolean True or False depending on whether the string is equal to the current password or not.
        
    class PasswordManager
    This class inherits from BasePasswordManage 
     methods
        set_password method that sets the user's password.
             Password change is successful only if:
                    - Security level of the new password is greater.
                    - Length of new password is minimum 6
        get_level method that returns the security level of the current password.
                 It can also check and return the security level of a new password passed as a string.
                   -level 0 - password consists of alphabets or numbers only.
                   -level 1 - Alphanumeric passwords.
                   -level 2 - Alphanumeric passwords with special characters.
