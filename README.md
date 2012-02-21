## WiMax Connection Balancce Checker for Bangladesh

Programs distributes with this package 'blionbal' and 'qubeebal' checks the remaining balance for Banglalion and Qubee WiMax ISPs. 
This is a program that runs on console and gives output on standard out. Its for those who uses limited plan. It will not work for unlimited plan users.

### Install 
Put both the *bal or the one whose connection you are using into a directory.  

### Running 
Run then like following,

    bash blionbal USERNAME PASSWORD # for Banglalion

And

    qubeebal USERNAME PASSWORD DATA-LIMIT  # for Qubee

Wait some time. It will  show the result in Console.

###Usage
When you run these programs it would requires some parameters. They are

- USERNAME user id for the connection
- PASSWORD password for the connection. Banglalion uses `123456` for every user.
- DATA-LIMIT data limit for your package. If your package has 12 GB data limit you can specify it as `"12 GB"` (with quotation) or `12GB` or `12,288 MB`  

**Note:** `qubeebal` has an extra parameter `DATA-LIMIT`.

The background color of the output is changed according to the size remaining. It can be configured by directly editing the executable. Try to find lines like following

    ## Put size in MB

    RED=256
    YELLOW=512
    GREEN=1024

It means it will show background color in RED if remaining size is less than 256 **MB**. If the size is between 255-511, color will be yellow. For the rest Color will be green(default), Remember, the size specified here is in **MB**. When you edit dont put any spaces (` `) arround `=` sign.

