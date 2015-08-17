# PasswordProject

This Java project that I have created allows a person to create a password and then validate its contents. 

Conditions:
- Password must be of a valid length and contain at least one number.
- Keep a history of recently used passwords. If a new one is created, it cannot be one that has been used recently.
- The password will expire at a given point in time and the user must be notified.
- Each password must have a maximum number of uses before it expires.
- When a new password is created, it must be encrypted. This is done by the following steps:
  1. Swap the first and last halves of the original password string.
  2. Reverse the order of all remaining characters.
  3. Perform a bitwise AND operation on the bits of each character of the encrypted password
      with those of the corresponding character in the original password.
  4. Append a hash code of the original password to the end of the encrypted password.
