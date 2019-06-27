# tmux install and setting file

## Install tmux

Reference URL : https://qiita.com/ha4gu/items/aebe9207904f52ee4fb6

### 1. Install required packages.
```bash
sudo apt update
sudo apt install git automake bison build-essential pkg-config libevent-dev libncurses5-dev

```

### 2. Download source code.
```bash
cd /usr/local/src/
git clone https://github.com/tmux/tmux
```

### 3. Build
```bash
cd ./tmux/
./autogen.sh
./configure --prefix=/usr/local
make
```

### 4. Install and confirmation
```bash
sudo make install
which tmux  # current directory is `/usr/local/bin/tmux`
tmux -V     # tmux next-3.1 (@2019/062/7)
```

