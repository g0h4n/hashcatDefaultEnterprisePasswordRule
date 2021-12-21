# hashcatDefaultEnterprisePasswordRule

Here is a **hashcat rule** for building a list of passwords. These are the formats I've seen most often in companies.

# How to use it?🔨

Create one file named **wordlist.txt** with for example the name of your target company:

```
google
```

```bash
wget https://raw.githubusercontent.com/g0h4n/hashcatDefaultEnterprisePasswordRule/main/hashcatDefaultEnterprisePasswordRule.rule
hashcat -r hashcatDefaultEnterprisePasswordRule.rule wordlist.txt --stdout > passwords.txt
```

<img src="./src/passwords.gif" alt="passwords list" />

Now you can use **passwords.txt** to try to crack a hash.⚙️