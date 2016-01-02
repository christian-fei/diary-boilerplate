diary-boilerplate
=================

this repo serves as a boilerplate for an encrypted diary with [GPG](https://en.wikipedia.org/wiki/GNU_Privacy_Guard).

you can start writing your own by following these steps:

1) Fork this repo, rename it at your needs.

2) Create a file called diary.md (it is ignored in .gitignore)

3) Write your diary and when you're done, encrypt the file with

```
gpg --symmetric --cipher-algo aes256 diary.md
# or
opt/encrypt
```

---

When you change computer or want to read the diary from another client, you can decrypt it with

```
gpg --decrypt diary.md.gpg > diary.md
# or
opt/decrypt
```
