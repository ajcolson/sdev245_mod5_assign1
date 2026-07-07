# SDEV245 Module 5 Assignment 1

Question Responses:
1.	Although this question has the heading “Broken Access Control”, the code in this question doesn't specify or have sufficient context to suggest if the requested information is privileged and requires any authentication action. Therefore, the only item of note here is to make sure we sanitize the user provided input data. We’ll assume SomeSanitizerFunc handles this. See: https://owasp.org/Top10/2025/A01_2025-Broken_Access_Control/
2.	Although this question has the heading “Broken Access Control”, as with question 1, the code in this question doesn't specify or have sufficient context to suggest if the requested information is privileged and requires any authentication action. Again, we should just sanitize the user input and then proceed. We’ll assume SomeSanitizerFunc handles this. See: https://owasp.org/Top10/2025/A01_2025-Broken_Access_Control/
3.	In this code, we should choose a different hashing algorithm. SHA256 is better than MD5. See: https://owasp.org/Top10/2025/A04_2025-Cryptographic_Failures/
4.	Again, we choose a different hashing algorithm. SHA256 is better than SHA1. See: https://owasp.org/Top10/2025/A04_2025-Cryptographic_Failures/
5.	We should sanitize the user’s input data to make sure we prevent any text that could be interpreted as SQL code and in some way escape it. We’ll assume SomeSanitizerFunc handles this. See: https://owasp.org/Top10/2025/A05_2025-Injection/
6.	We should sanitize the user’s input data to make sure we prevent any text that could be interpreted as NoSQL code and in some way escape it. We’ll assume SomeSanitizerFunc handles this. See: https://owasp.org/Top10/2025/A05_2025-Injection/
7.	If we let anonymous users attempt to reset passwords for their accounts, we should implement some security token(s) that are unique to each user that must be passed with our form. We’ll assume ValidUserTokenChecker implements a way to check if a token provided is valid and remove the token from use if successful. See: https://owasp.org/Top10/2025/A06_2025-Insecure_Design/
8.	If we are going to use a CDN for some library code, we should include an integrity attribute that allows the browser to verify that the requested file hasn’t been modified.
See: https://owasp.org/Top10/2025/A08_2025-Software_or_Data_Integrity_Failures/
9.	We should check if the user provided data is a valid URL format, sanitize if needed, and potentially check if the URL is whitelisted if we choose to implement a whitelist feature. See: https://owasp.org/Top10/2025/A08_2025-Software_or_Data_Integrity_Failures/
10.	We shouldn’t try to compare passwords in plaintext, instead we should compare against a password hash. See: https://owasp.org/Top10/2025/A07_2025-Authentication_Failures/
