------------
**Visit GitHub Repo**: [https://github.com/diggajupadhyay/tmpmail](https://github.com/diggajupadhyay/tmpmail "https://github.com/diggajupadhyay/tmpmail")

> tmpmail is a command line utility written in POSIX sh that allows you to create a temporary email address and receive emails to the temporary email address. It uses 1secmail's API to receive emails.tmpmail is a command line utility written in POSIX sh that allows you to create a temporary email address and receive emails to the temporary email address. It uses 1secmail's API to receive emails.

------------


#### Run the Image
- `docker run -it --rm diggajupadhyay/tmpmail`

OR,

- `docker run -it --rm diggajupadhyay/tmpmail:v0.0.2`


------------
#### Examples

- Create random email
```shell
$ tmpmail --generate
xoithrjagpx@1secmail.net
```
- Create custom email
```shell
$ tmpmail --generate mycustomemail@1secmail.com
mycustomemail@1secmail.com
```
- View the inbox
```shell
$ tmpmail
[ Inbox for wdebivbyjor@1secmail.com ]
83414443   username@example.com   Test Email
```
- View the email
```shell
$ tmpmail 83414443
```
- View the most recent email
```shell
tmpmail -r
```
- View emails as pure text
```shell
$ tmpmail -t 83414443
To: wdebivbyjor@1secmail.com
From: username@example.com
Subject: Test Email
Hello World
[Attachments]
https://is.gd/aBCdEf [apple.jpg]
https://is.gd/AbCDeF [ball.jpg]
```
------------