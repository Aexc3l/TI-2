The unit tests for Single Checksum and Dual Checksum are presented below. These tests in turn are intended to validate the following objectives:

- **Data Integrity**: We run the project with a test dataset containing a variety of data, ensuring that the calculated Checksum values are consistent with expectations.

- **Performance**: We run tests on datasets of different sizes to evaluate the performance of the algorithms. Making sure that the execution time is acceptable even for large datasets.

- **Resilience**: We run the project with datasets containing extreme values or unexpected data, making sure that the algorithms handle these cases without errors.
- **Size**: Entries are categorized by the type of string that enters and its size as follows
	-  Toy, 𝑛 < $10^2$.
	- Small, $10^2$ ≤ 𝑛 < $10^4$.
	- Medium, $10^4$ ≤ 𝑛 < $10^5$
	- Large, 𝑛 ≥ $10^6$.


**Single Checksum Unit Tests (1.1)**
The unit tests for Single Checksum and Dual Checksum are presented below. These tests in turn are intended to validate the following objectives:

  

- **Data Integrity**: We run the project with a test dataset containing a variety of data, ensuring that the calculated Checksum values are consistent with expectations.

  

- **Performance**: We run tests on datasets of different sizes to evaluate the performance of the algorithms. Making sure that the execution time is acceptable even for large datasets.

  

- **Resilience**: We run the project with datasets containing extreme values or unexpected data, making sure that the algorithms handle these cases without errors.

- **Size**: Entries are categorized by the type of string that enters and its size as follows

- Toy, 𝑛 < $10^2$.

- Small, $10^2$ ≤ 𝑛 < $10^4$.

- Medium, $10^4$ ≤ 𝑛 < $10^5$

- Large, 𝑛 ≥ $10^6$.

  
  

**Single Checksum Unit Tests (1.1)**


| Test Description | Input Size | Input | Expected Outcome |
|------------------|-------------|--------|------------------|
| **Integrity Tests (Size Toy)**|| | |
| Test: Uppercase Text | Toy |`"HELLO"`| |
| Test: Lowercase Text | Toy | `"world"`| |
| Test: Mixed Text | Toy | `"MixEd123TeXT"` | |
| Test: Text with Spaces| Toy | `"Spaced Text Input"`| |
| Test: Text with Symbols | Toy | `"!@#$%^&*_-+=/\\| |
| Test: Text with Numbers| Toy | `"2023 is the year!"`| |
| **Integrity Tests (Size Small)**| | |
| Test: Uppercase Text| Small |`"HELLO, WORLD!"`| |
| Test: Lowercase Text| Small |`"hello, world!"`| |
| Test: Mixed Text | Small |`"Text123MixedWithNumbers"`| |
| Test: Text with Spaces| Small | `"Spaced Text Input for Test"`| |
| Test: Text with Symbols| Small |`"!@$SpecialSymbols*_-+=/\\`| |
| Test: Text with Numbers| Small | `"Numbers1234567890InTheText"`| |
| **Integrity Tests (Size Medium)**||| |
| Test: Uppercase Text | Medium |`"This is a Medium-Sized Input for testing Checksum Algorithm."`| |
| Test: Lowercase Text | Medium | `"this is a medium-sized input for testing checksum algorithm."`| |
| Test: Mixed Text| Medium | `"This is a mixed input with Numbers and Letters like 9876ABCD."` | |
| Test: Text with Spaces| Medium | `"Spaced Medium Size Text Input for Testing Checksum Algorithm."`| |
| Test: Text with Symbols| Medium| `"Medium Sized Text Input with Symbol !@#$%^&*_-+=/@$--.{+}¿#"@@"` | |
| Test: Text with Numbers| Medium| `"Second medium-sized input with numbers from this 12345, 67890."` | |
| **Integrity Tests (Size Big)**||| |
| **Uppercase Text**| Big | `"This is a BIG and Massive input with CAPITAL LETTERS, numbers, and special characters"`| |
| **Lowercase Text**| Big | `"this is a big and massive input with capital letters, numbers, and special characters."` | |
| **Mixed Text** | Big | `This is a BIG and Massive input with 123455678906589435 numbers, and special characters"`| | |
| **Text with Spaces** | Big | `This is a big and massive input with Spaces and Letters, no numbers, and more spaces"` | |
| **Text with Symbols**| Big | `This is a BIG and Massive input with !@#$%^&*_-+=/@$--.{+}¿#"@@!@#$%^&*_-+=/@$--.{+}¿"` | | |
| **Text with Numbers**| Big | `"This is a very long input with lots of numbers and large numbers like 12345678901234567890."` | |



