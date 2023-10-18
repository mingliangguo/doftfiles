# README

## encrypt

When run `yadm encrypt` on MacOS, it throws errors like 

```bash
gpg: problem with the agent: Inappropriate ioctl for device
gpg: error creating passphrase: Operation cancelled
gpg: symmetric encryption of '[stdin]' failed: Operation cancelled
```

To workaround it, run the following export:

```bash
export GPG_TTY=$(tty)
```
