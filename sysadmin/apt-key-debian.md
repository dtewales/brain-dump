# apt-key Depreciation

With the depreciation, removal of old repo signing keys is now achievable with gpg.

## List Keys
```bash
gpg --no-default-keyring --keyring /etc/apt/trusted.gpg --list-keys --with-fingerprint
```

## Key Removal
```bash
gpg --no-default-keyring --keyring /etc/apt/trusted.gpg --delete-key "[ key identifier from --list-keys ]"
```