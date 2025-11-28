# hashcatDefaultEnterprisePasswordRule

Here is a **Hashcat rule** designed to generate password candidates based on formats commonly observed in enterprise environments.

# How to use it?🔨

Create a file named wordlist.txt containing, for example, the name of your target company:

```
google
```

Obviously, using a Hashcat rule requires that Hashcat is already installed… 🤷‍♂️

```bash
wget https://raw.githubusercontent.com/g0h4n/hashcatDefaultEnterprisePasswordRule/main/hashcatDefaultEnterprisePasswordRule.rule

hashcat -r hashcatDefaultEnterprisePasswordRule.rule wordlist.txt --stdout > passwords.txt
```

<img src="./src/passwords.gif" alt="passwords list" />

You can now use passwords.txt to attempt cracking hashes. ⚙️