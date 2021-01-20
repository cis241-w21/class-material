# Minilab 0

The purpose of today is to make sure that everyone can access
using ssh since we'll be accessing EOS frequently.

## Tasks

1. Remember your account info
   * Everyone should have an account
     * Likely got the account the first time you took a CIS class
     * If this is your first one, check your email
   * Username will be the same as your gvsu login name
   * Password is either whatever was sent in the email when your
     account was first created or whatever you changed it to
   * If you never got an email or don't know your account info,
     contact hpcsupport@gvsu.edu

2. Open up a terminal:
   * On Mac:  spotlight search for terminal - you'll likely want
     to set to keep in the dock since we'll use it so much
   * On Windows:  This is the WSL.  Make sure you've followed the
     [instructions to install WSL](wsl-guide.md).  Click the start button and search for
     Ubuntu.  Select it and a terminal should open.

3. Start up the VPN.  Follow the
   [VPN instructions](https://www.gvsu.edu/it/downloading-installing-and-setting-up-pulse-secure-for-222.htm).
   You only need to download/install 1x.  After that, just jump to step 7.

4. Try connecting via ssh.  Type into the terminal
   `ssh userid@35.39.165.xx` where `xx` is a number between 61 and 91.

   Each of these #s correspond to a different physical computer in the EOS lab (these are for eos01
   through eos31).

   * If for some reason you get an error like "Network is unreachable",
     just try a different number (someone probably shut down that computer).
   * If you see a question about authenticity/fingerprint, type `yes`.  Theoretically,
     you are supposed to check that the fingerprint matches by comparing to what is
     published elsewhere, to make sure someone else
     isn't posing as that machine, but the fingerprints are not even published nowadays.
   * Note:  if you are ever physically in EOS (maybe someday!), don't shutdown the computers
     because people might be on them remotely.

5. Type 'exit' to disconnect from the remote machine and go back to your computer.

6. The long numbers like `35.39.165.61` are the ip addresses of the EOS computers.
   Since it's a pain to remember these, these computers are instead given hostnames
   on the gvsu domain.  Together, this means these computers have a *fully qualified domain name*.
   For all of the EOS machines, these are `eosXX.cis.gvsu.edu` where `XX` is 01 through 31.

   So, instead of running `ssh userid@35.39.165.xx` we should be able to run
   `ssh userid@eosXX.cis.gvsu.edu`. 

   
   This is where the process splits depending on whether you are on Mac/Linux or
   WSL.  Note, there's **no** reason the process should be different, but WSL is 
   still fairly new and occasionally buggy.

   * Mac/Linux users: `run userid@eosXX.cis.gvsu.edu` where `XX` is some number
     between 01 and 31.  Then, type `exit` to disconnect from the remote machine.
   * Windows users:
     1. run `cd ~/.ssh`
     2. run `vim config`
     3. Type `i`
     4. Type the following lines in this order:
        ```
        Host eos01.cis.gvsu.edu
        Hostname 35.39.165.61
        Host eos02.cis.gvsu.edu
        Hostname 35.39.165.62
        ``` 
        03, ... 31 instead of 01 or 02 in which
        case you would want to use the corresonding number
        (.63, ..., .91)
     5. Press ESC
     6. Type `:wq` then press ENTER
     7. Run `ssh userid@eos01.cis.gvsu.edu` (or one of the EOS #s you typed a minute ago).
     8. Type `exit` to disconnect from the remote machine

7. Optional:  change your password
   1. ssh into any eos machine
   2. Run `passwd` and follow the instructions to change your password
   3. Type `exit` to disconnect from the remote machine