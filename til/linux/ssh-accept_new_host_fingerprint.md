# Accept new host fingerprint

Sometimes it happens that the target host, where you are trying to connect to, was re-installed. In that case your attempt to connect may be refused by your client - simply the host fingerprint has changed and it's fingerprint record in `known_hosts` doesn't match the current one (your client then thinks it might be man-in-the-middle attack).

If you are sure that it's OK to accept new fingerprint, the easiest way is:

```
ssh-keygen -R <hostname>
```

This will force update of `known_hosts` with new fingerprint of specified `<hostname>`.