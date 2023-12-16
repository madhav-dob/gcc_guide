
# One Stop guide for gcc

Here, I have mentioned commands to install and update gcc compiler
## Install GCC

### Method 1: Using apt

1. **Install GCC:**
```bash
sudo apt install gcc
```

This will install the default version of GCC available in the Ubuntu repository.

2. **Verify the Installation:**
```bash
gcc --version
```

This command will display the installed GCC version.

### Method 2: Installing a Specific Version

If you need a specific version of GCC, you can install it using the following steps.

1. **Check Available Versions:**
```bash
apt search gcc
```

2. **Install a Specific Version:**
```bash
sudo apt install gcc-<version_number>
```
Replace `<version_number>` with the specific version you want to install (e.g., gcc-9, gcc-10, etc.).

3. **Verify the Installation:**
```bash
gcc --version
```
## Changing GCC version
### Go to this directory and list the installed gcc versions
```bash
cd /usr/bin
ls grep | gcc
```
### Remove the existing version :
```bash
rm gcc
```
### Update the version:
```bash
cp gcc<version> gcc
```
## Update GCC

To update GCC to the latest available version:

1. **Update GCC:**
```bash
sudo apt upgrade gcc
```

This command will upgrade GCC to the latest version available in the Ubuntu repository.

2. **Verify the Updated Version:**
```bash
gcc --version
```

## Additional Notes

- Make sure you have administrative privileges (`sudo`) to execute these commands.
- The default repositories might not always have the latest GCC version. Consider using PPAs or other sources for newer versions.
