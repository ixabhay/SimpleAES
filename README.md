Usage:

string decryptedBalance = "99";
        try{
            decryptedBalance = AES256.Decrypt(savedDataSO.GetValue("Balance"), key);
            Debug.Log("Decrypted balance: " + decryptedBalance);
        }catch{
            Debug.Log("Error decrypting balance: " + decryptedBalance);
        }


string encryptedBalance = AES256.Encrypt(currentBalance.ToString(), key);
        Debug.Log("Encrypted balance: " + encryptedBalance);
