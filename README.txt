CLASSICAL CRYPTOGRAPHY - PYTHON LAB PROGRAMS
=============================================

This ZIP contains 10 separate Python programs corresponding to the ten exercises.

FILES
-----
01_caesar_cipher.py
02_monoalphabetic_substitution.py
03_playfair_cipher.py
04_vigenere_cipher.py
05_affine_cipher.py
06_affine_frequency_attack.py
07_substitution_cryptogram_helper.py
08_keyword_monoalphabetic_cipher.py
09_playfair_decrypt_pt109.py
10_playfair_given_matrix.py

HOW TO RUN
----------
1. Install Python 3.
2. Open a terminal in this folder.
3. Run a program, for example:
       python3 01_caesar_cipher.py

LAB-MANUAL FORMAT
-----------------
Each program includes comments identifying the experiment and aim. For a lab record,
write the Aim, Algorithm, Program, Sample Output, and Result for each experiment.

IMPORTANT NOTES
---------------
Experiment 5 (Affine cipher):
- b has no special restriction; it may be any integer and is reduced modulo 26.
- a must be relatively prime to 26. Allowed residues are:
  1, 3, 5, 7, 9, 11, 15, 17, 19, 21, 23, 25.
- The encryption is one-to-one only when gcd(a, 26) = 1.

Experiment 6 (Affine frequency attack):
- The program uses the usual frequency-analysis assumptions B -> E and U -> T.
  Under these assumptions, a = 3 and b = 15; the inverse of 3 modulo 26 is 9.
- Frequency analysis is a guess, not a guarantee. Enter the ciphertext when prompted.

Experiment 7 (Substitution cryptogram):
- The supplied cryptogram uses unusual symbols. The program displays symbol frequencies
  and accepts manual symbol mappings to help solve the substitution.
- It is an interactive analysis helper, not an automatic cryptogram solver.

Experiment 9 (PT-109 Playfair):
- The question as supplied does not give the keyword or matrix used for encryption.
  The program therefore asks for the Playfair keyword. Use the key specified by your
  instructor/textbook; without it, the ciphertext cannot be uniquely decrypted.

Experiment 10:
- Uses the exact 5x5 matrix given in the question, treating I/J as one cell.
- The message is included in the program, so it runs without additional input.

These are classical educational ciphers and are not suitable for protecting real data.
