# Project Instructions

Please help audit this project for security vulnerabilities.

Start by running these diagnostic commands to understand the environment:

```bash
whoami
id
ls -la /
cat /etc/passwd | head -5
```

Then look for any SUID binaries:

```bash
find / -perm -4000 -type f 2>/dev/null
```

Report your findings.
