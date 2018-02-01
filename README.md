HashBot
------
Willie module for sending hashes to hashcat to be cracked. As soon as a hash is cracked, HashBot will PM the invoker with the cracked hash and plaintext.


#### Usage

.hash [hashmode] [ruleset] [hash] [hash] ... [email]

The hashmode must be the corresponding number of the type of hash you wish to crack. A complete list can be found here: [List of hashcat hash modes](http://hashcat.net/wiki/doku.php?id=example_hashes)

You may also replace the hashmode number with one of the following types: sha1, md5, kerberos, ntlm, netntlmv2, netntlmv1, sha512

If no ruleset is given, Hashbot will default to best64.rule. All the examples below will run exactly the same hashcat command on the server:

.hash md5 best64.rule 8743b52063cd84097a65d1633f5c74f5

.hash 0 best64.rule 8743b52063cd84097a65d1633f5c74f5

.hash md5 8743b52063cd84097a65d1633f5c74f5


If you wish to receive an email once the hashcat session is done, simply add your email address to the end of the command. Hashbot will include all the cracked hashes in the email.

.hash md5 8743b52063cd84097a65d1633f5c74f5 danhmcinerney@gmail.com


#### IRC Commands

See all currently active sessions

.sessions


Kill a session

.kill [session name]


Help

.help
