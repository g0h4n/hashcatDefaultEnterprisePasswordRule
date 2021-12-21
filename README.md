# hashcatDefaultEnterprisePasswordRule

Here is a **hashcat rule** for building a list of passwords. These are the formats I've seen most often in companies.

# How to used it?🔨

Create one file named **wordlist.txt** with for example the name of your target company:

```
google
```

```bash
wget hashcatDefaultEnterprisePasswordRule.rule
hashcat -r hashcatDefaultEnterprisePasswordRule.rule wordlist.txt --stdout > passwords.txt
```

<img src="./src/passwords.gif" alt="passwords list" />

Now you can use **passwords.txt*** to try to crack a hash.⚙️