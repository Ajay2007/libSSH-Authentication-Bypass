# libSSH-Authentication-Bypass
Spawn to shell without any credentials by using CVE-2018-10933

Information about CVE-2018-10933 by libSSH : https://www.libssh.org/security/advisories/CVE-2018-10933.txt

Bugfix Release by libSSH : https://www.libssh.org/2018/10/16/libssh-0-8-4-and-0-7-6-security-and-bugfix-release/

## Create a vulnerable ssh server or directly use tool to bypass remote server:

Download, uncompress and build the vulnerable libSSH Version : https://www.libssh.org/files/0.7/libssh-0.7.4.tar.xz

And then compile and run libSSH on your own server with ssh.

```
PWD: /libssh-0.7.4/build/examples/samplesshd-cb
./samplesshd-cb --dsakey==yourdsakey 127.0.0.1 --port=2222
```


## libSSH Authentication Bypass with two different tools
**If you have got any fake ssh keys use the second bypasswithfakekey.py**
```
pip install -r requirements.txt
If paramiko==2.0.8 doesn't works try : pip install paramiko==2.4.2
```
# Usage: 
```
python libsshauthbypass.py --help
python bypasswithkey.py --help
```

## Shodan.io libSSH

![](https://i.imgur.com/SWEfcGR.png)
