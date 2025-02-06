# Longest Compound Word Finder

## Overview
This Java program reads a list of words from a file and determines the longest and second longest compound words. A compound word is defined as a word that can be formed by concatenating shorter words from the same list.

## Features
- Reads words from an input file.
- Identifies the longest and second longest compound words.
- Uses dynamic programming for efficient word formation checking.
- Utilizes a `HashSet` for fast word lookups.
- Outputs the processing time taken to find the results.

## Prerequisites
- Java Development Kit (JDK) 8 or later
- An input file containing a list of words (one per line) named `Input_01.txt`

## How to Run
1. Compile the Java program:
   ```sh
   javac LongestCompoundWord.java
   ```
2. Run the compiled program:
   ```sh
   java LongestCompoundWord
   ```

## Input File Format
The program expects an input file (`Input_01.txt`) with words listed line by line. Example:
```
cat
cats
catsdogcats
dog
dogcatsdog
rat
ratcatdogcat
```

## Expected Output
The program prints:
```
Longest Compound Word: ratcatdogcat
Second Longest Compound Word: catsdogcats
Time taken to process file Input_01.txt: X milliseconds
```

## Code Explanation
- **`readWordsFromFile(String fileName)`**: Reads words from a given file.
- **`findLongestCompoundWords(List<String> words)`**: Identifies the longest and second longest compound words.
- **`canFormWord(String word, Set<String> wordSet)`**: Uses dynamic programming to check if a word can be formed using other words in the set.

## Performance Considerations
- Uses a `HashSet` for O(1) lookup time.
- Sorts words in descending order by length to optimize processing.
- Uses a dynamic programming approach for efficient substring checking.

## Example Execution
```sh
javac LongestCompoundWord.java
java LongestCompoundWord
```
