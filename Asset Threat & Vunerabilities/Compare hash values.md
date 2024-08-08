# Compare Hash Values

## Description
As a security analyst, one of the security controls we can implement is hashing. It produces a code that cannot be decrypted. It works by uniquely identifying the contents of a file, later
known as a unique identifier (hash value or digest). For example, a malicious program may mimic an original program. If one code line is different from the original program, it produces a different hash value. Security teams can then identify the malicious program and work to mitigate the risk.

## Generate Hashes
First, `ls` command shows the files within the directory. We have two files and we would like to show the contents of them (`cat`). We could see from the picture below that the contents of both files appear to be identical.

![image](c:\Users\sanil\Desktop\Img1.png)

We can find if the files are really different or not by using the `sha256` command. From the picture below we can see both files have different hash values.

![image](c:\Users\sanil\Desktop\img2.png)

## Compare Hashes Files
Let’s generate the hash of the `file1.txt` and `file2.txt` to a new file for `file1hash` and `file2hash` respectively.  

![image](c:\Users\sanil\Desktop\img3.png)

Inspect the contents of them by using `cat` commands. Last but not least, compare both files by using `cmp` command.

![image](c:\Users\sanil\Desktop\img4.png)

![image](c:\Users\sanil\Desktop\img5.png)

## Summary
Though the contents of both files appear to be identical, only hash values of each file that can determine if they are the same or not.