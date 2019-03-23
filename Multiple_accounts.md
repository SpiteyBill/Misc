# Using multiple github accounts on one PC

## Using Tortoise Git

Assume you have two github accounts:

- __name1__
- __name2__

and you have two repositories, cloned into different directories:
- __repo1__ (under name1)
- __repo2__ (under name2)

What happens is, the credentials of one repo can conflict with the other, thus affecting pulling and pushing.

Change these settings for each repository as shown below (pictures show only for name1/repo1:

1. **Use HTTPS encryption.** - TortoiseGit Settings > Git > Remote > Origin > URL
2. **Set Git credentials** - TortoiseGit Settings > Git > Remote > Origin > URL
3. **Save username and password** - To avoid having to put in your username and password again and again (if it is your own PC), then open git bash in both repos, and type:
```
git config user.name "name1"
git config user.password "password_name1"
```
Please note the username and password need to be in "quotes".
