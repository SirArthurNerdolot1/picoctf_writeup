# Collaborative Development
## Description
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together? You can download the challenge files here:[challenge.zip](https://artifacts.picoctf.net/c_titan/178/challenge.zip)
## Solution
Unzipping the file we get:
```
❯ ls
challenge.zip  drop-in
```
On opening drop-in:
```
❯ cd drop-in
                                                                                                                     
❯ ls
flag.py
```
On seeing the python file, we try to run it once:
```
❯ python3 flag.py
Printing the flag...
```
It doesn't printf the flag so we have to open the python script:
```
printf("Printing the flag... ")
```
So, it has no flag given inside.
We look for other branches in the repo:
```
❯ git branch -a
  feature/part-1
  feature/part-2
  feature/part-3
* main

❯ git checkout feature/part-1
Switched to branch 'feature/part-1'
                                                                                                                     
❯ ls
flag.py
                                                                                                                     
❯ python3 flag.py
Printing the flag...
picoCTF{t3@mw0rk_  
❯ git checkout feature/part-2
Switched to branch 'feature/part-2'
                                                                                                                     
❯ ls
flag.py
                                                                                                                     
❯ python3 flag.py
Printing the flag...
m@k3s_th3_dr3@m_       

❯ git checkout feature/part-3
Switched to branch 'feature/part-3'
                                                                                                                     
❯ ls
flag.py
                                                                                                                     
❯ python3 flag.py
Printing the flag...
w0rk_6c06cec1}
```
On combining the strings, we get:
```
picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_6c06cec1}
```
                    
                    


