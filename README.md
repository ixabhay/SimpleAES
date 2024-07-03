# SimpleAES for Unity or any C# program

To decrpyt an encrypted data:
```csharp
string decryptedBalance = "99";
        try{
            decryptedBalance = AES256.Decrypt(savedDataSO.GetValue("Balance"), key);
            Debug.Log("Decrypted balance: " + decryptedBalance);
        }catch{
            Debug.Log("Error decrypting balance: " + decryptedBalance);
        }
```

To encrypt a data:
```csharp
string encryptedBalance = AES256.Encrypt(currentBalance.ToString(), key);
        Debug.Log("Encrypted balance: " + encryptedBalance);
```



