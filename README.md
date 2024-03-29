# mybel
Notification rings using the terminal bel.

It's just a simple script to notify you if a command has finished running.

## Usage
`<any command> ; <mybel[1-3]>`

### Example
`dd if=... of=... bs=... ; mybel1`

And you will hear if the dd has finished. ;)

## Installation
- You can either [download](https://github.com/tamas646/mybel/raw/main/mybel_1.0.0_all.deb) and install the deb package or use the source code and setup it yourself.

- If you wish, you can install it from my apt repository too:

  ```sh
  sudo echo "deb [signed-by=/usr/share/keyrings/ptamas-pub.gpg] http://apt.ptamas.hu/main/ ./" > /etc/apt/sources.list.d/apt.ptamas.list
  wget -qO - https://apt.ptamas.hu/ptamas-pub.gpg | gpg --dearmor | sudo tee /usr/share/keyrings/ptamas-pub.gpg > /dev/null
  apt update && apt install mybel
  ```
