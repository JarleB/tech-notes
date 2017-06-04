Setup new gpg keys, backup and load onto yubikey according to https://research.kudelskisecurity.com/2017/04/28/configuring-yubikey-for-gpg-and-u2f/

Configure and allow  ssh to access gpg-keys 
https://incenp.org/notes/2015/gnupg-for-ssh-authentication.html

Many guides for setting up ssh-auth with gpg-cards is outdated wrt. the need for setting GPG_AGENT_INFO. This is obsolete since gpg 2.1 
https://unix.stackexchange.com/questions/188668/how-does-gpg-agent-work

ssh is confused with ttys. (Pinentry appears in wrong tty ) Fix with  "echo UPDATESTARTUPTTY | gpg-connect-agent" 
https://www.gnupg.org/documentation/manuals/gnupg/Common-Problems.html 

unblock pin
https://github.com/ruimarinho/yubikey-handbook/blob/master/openpgp/troubleshooting/gpg-failed-to-sign-the-data.md

See also
https://www.yubico.com/support/knowledge-base/categories/articles/use-yubikey-openpgp/
https://developers.yubico.com/PGP/SSH_authentication/
https://www.esev.com/blog/post/2015-01-pgp-ssh-key-on-yubikey-neo/
https://spin.atomicobject.com/2014/02/09/gnupg-openpgp-smartcard/
https://alexcabal.com/creating-the-perfect-gpg-keypair/
https://developers.yubico.com/PGP/Card_edit.html
http://techhappy.co.nz/2016/05/yubikey-better-security-convenience/
