# Sentence Analysis Algorithm

## Description

This algorithm analyzes a given sentence by computing the following:

- The **length** of the sentence (number of characters, including spaces and punctuation).
- The **number of words** in the sentence.
- The **number of vowels** present in the sentence.

## Variables Used

- **sentence**: Stores the input sentence.
- **length_counter**: Counts the total number of characters in the sentence.
- **word_counter**: Counts the number of words in the sentence (initially set to 1).
- **vowel_counter**: Counts the number of vowels in the sentence.
- **vowels**: A string containing all vowels (both uppercase and lowercase) for easy comparison.

## Algorithm Steps

1. **Initialize variables**:

   - Accept an input sentence.
   - Set `length_counter = 0`, `word_counter = 1`, and `vowel_counter = 0`.
   - Define `vowels = "aeiouAEIOU"`.

2. **Iterate through each character in the sentence**:

   - Increment `length_counter` by 1.
   - If the character is found in the `vowels` list, increment `vowel_counter`.
   - If the character is a space, increment `word_counter` (as spaces separate words).

3. **Output the results**:
   - Print the length of the sentence.
   - Print the number of words in the sentence.
   - Print the number of vowels in the sentence.

## Example Execution

### Input:

```
I see a crystal raindrop fall and the beauty of it all.
```

### Output:

```
Length of the sentence: 51
Number of words in the sentence: 13
Number of vowels in the sentence: 18
```

## Complexity Analysis

- **Time Complexity**: O(n) (where n is the length of the sentence, as we iterate through it once).
- **Space Complexity**: O(1) (as we use a fixed number of variables regardless of input size).

## Notes

- This algorithm assumes words are separated by **single spaces** and does not account for multiple consecutive spaces or punctuation marks.
- The accuracy of word counting can be improved by handling edge cases such as trailing spaces or special characters.

## Future Improvements

- Consider handling punctuation marks separately.
- Account for multiple spaces between words.
- Allow for more flexible vowel detection (e.g., including accented vowels).
