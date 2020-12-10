# greyscanner

greytrapping daemon to complement OpenBSD spamd

## DESCRIPTION

greyscanner complements OpenBSD spamd(8) greylisting by applying
additional heuristics to greylisted hosts. Additional heuristics
include: confirm senders email address is valid, confirm existence of
the senders MX or A record in DNS, confirm recipient address(es) is
valid, and more. Offending hosts are flagged as 'trapped' in the spamd
database.

## FILES

/etc/mail/greyscanner.conf optional config file

## SEE ALSO

[spamd(8)](https://man.openbsd.org/spamd), [spamdb(8)](https://man.openbsd.org/spamdb)

## HISTORY

Bob Beck created greyscanner in 2006.  Jim Razmus II revised the
program, added documentation, and packaged it for OpenBSD in 2009.
