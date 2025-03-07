# orapass

Oracle Password Management using Oracle Wallet Manager

orapass is a command-line tool for securely storing and retrieving credentials using an Oracle Wallet. Use orapass to create a wallet in /opt/oracle/orapass, be sure to back it up.

# Installation
```
cp orapass /usr/local/bin/orapass
chmod +x /usr/local/bin/orapass
```

# Usage
Required first step, this creates /opt/oracle/orapass and sets up Oracle Wallet.

```
orapass init
````


# Store a Credential
Example stores admin/somesecurepw for the ORCL database.
```
orapass put ORCL admin somesecurepw
```


# List Stored Credentials
```
orapass list

Example Output:
1: ORCL_admin 
2: HR_user

```
 
# Retrieve Password
```
orapass get ORCL admin
```



