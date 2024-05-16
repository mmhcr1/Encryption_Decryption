# Encryption_Decryption

Importing Necessary Modules: The code begins by importing the string module, which provides various string constants like string.ascii_lowercase, containing all lowercase letters of the alphabet.

Defining Variables:
alphabets variable stores all lowercase letters of the alphabet twice. This is to handle wrapping around when shifting beyond 'z'.

sentence variable takes user input and converts it into lowercase letters, stored as a list.

what_to_do variable asks the user whether to encrypt, decrypt, or exit the program.

shift_number variable takes the number of positions each letter should be shifted.

end_program variable tracks whether the program should continue running.

Main Program Execution:
The program enters a while loop that continues until end_program becomes True.

If the user chooses encryption, it iterates through each character in the input sentence:
If the character is a space, it remains unchanged.

Otherwise, it finds the index of the character in the alphabets string, adds the shift number, and replaces the character with the shifted character.

If decryption is chosen, the process is similar, but it subtracts the shift number instead.

The resulting encrypted or decrypted sentence is then printed.

Handling Invalid Input:
If the user enters an invalid choice, it prompts the user to try again. If the user chooses not to try again, end_program becomes True, and the program ends.

Overall, this code is a simple implementation of the Caesar cipher, a basic encryption technique. The security of this encryption depends solely on the secrecy of the shift number. However, since the shift number is provided by the user and has a limited range, it can be easily decrypted through brute force or frequency analysis, making it relatively insecure for real-world applications.






