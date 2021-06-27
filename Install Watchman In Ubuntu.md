### Install watchman

---

```
sudo apt install libssl-dev autoconf automake libtool pkg-config python-dev
git clone https://github.com/facebook/watchman.git
cd watchman
git checkout v4.9.0  # the latest stable release
./autogen.sh
./configure
make
(if error
./configure --without-python  --without-pcre --enable-lenient
make)
sudo make install
```

### Verify

---

https://facebook.github.io/watchman/docs/cmd/version.html
