# Compare Hash Values

## Description
As a security analyst, one of the security controls we can implement is hashing. It produces a code that cannot be decrypted. It works by uniquely identifying the contents of a file, later
known as a unique identifier (hash value or digest). For example, a malicious program may mimic an original program. If one code line is different from the original program, it produces a different hash value. Security teams can then identify the malicious program and work to mitigate the risk.

## Generate Hashes
First, `ls` command shows the files within the directory. We have two files and we would like to show the contents of them (`cat`). We could see from the picture below that the contents of both files appear to be identical.

![Img1](https://github.com/user-attachments/assets/4352e296-5570-4f65-852c-1a588b2f3f0e)

We can find if the files are really different or not by using the `sha256` command. From the picture below we can see both files have different hash values.

![img2](https://github.com/user-attachments/assets/b5fecff9-55b6-4ff3-995b-b500c887dec2)

## Compare Hashes Files
Let’s generate the hash of the `file1.txt` and `file2.txt` to a new file for `file1hash` and `file2hash` respectively.  

![img3](https://github.com/user-attachments/assets/24bfcb73-842e-4c7c-a188-4d341a9a4bfb)

Inspect the contents of them by using `cat` commands. Last but not least, compare both files by using `cmp` command.

![img4](https://github.com/user-attachments/assets/5e0927cc-8413-4613-b88d-4a4d04bcddae)

![img5](https://github.com/user-attachments/assets/9f963d35-58d7-4d4a-a58c-9dd6cee48ebb)

## Summary
Though the contents of both files appear to be identical, only hash values of each file that can determine if they are the same or not.