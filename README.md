
def length_of_last_word(s):
    # Trim leading and trailing spaces
    trimmed_s = s.strip()

    # Initialize a variable to store the length of the last word
    last_word_length = 0

    # Iterate through the characters in the trimmed string
    for char in trimmed_s:
        # If the current character is a space, reset the last_word_length
        if char == ' ':
            last_word_length = 0
        else:
            # If the current character is not a space, increment last_word_length
            last_word_length += 1

    # Return the length of the last word
    return last_word_length









The logic of the code is:
    1.Trimming Spaces:
trimmed_s = s.strip(): This line removes leading and trailing spaces from the input string s. This is done to handle cases where there might be spaces before or after the words in the string.

2.Iterating Through Characters:
for char in trimmed_s:: This loop iterates through each character in the trimmed string.

3.Counting Word Length:
if char == ' ': last_word_length = 0: If the current character is a space, it resets the last_word_length to 0. This is because we want to start counting the length of a new word.
else: last_word_length += 1: If the current character is not a space, it increments the last_word_length. This is done to keep track of the length of the current word.

4.Returning the Result:
return last_word_length: Finally, the function returns the length of the last word, which has been calculated during the iteration.









The algorithm of the code is:

1.Input:
Take a string s as input.

2.Trim Spaces:
Trim leading and trailing spaces from the string and store the result in trimmed_s.

3.Initialize Variables:
Initialize a variable last_word_length to store the length of the last word.

4.Iterate Through Characters:
For each character char in the trimmed string:
If char is a space:
Reset last_word_length to 0, indicating the start of a new word.
If char is not a space:
Increment last_word_length, counting the length of the current word.

5.Return Result:
Return the value of last_word_length as the length of the last word in the string.

6.Output:
The returned value represents the length of the last word in the original string.
