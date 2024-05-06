# hyperledger_docs

## Installation:

  ## Pre-requisites:
  ```
  docker
  docker Compose
  cURL
  jq
  golang
  git
  ```
For installing `jq`, run `sudo apt install jq`, if you face some issues, eg: `Unable to fetch some archives`, run:
```
sudo apt-get install jq --fix-missing
```

# Install hyperledger fabric samples:
```
$ mkdir hyperlegder-samples
$ cd hyperledger-samples
$ curl -sSLO https://raw.githubusercontent.com/hyperledger/fabric/main/scripts/install-fabric.sh && chmod +x install-fabric.sh #to give executable permissions to the shell script.
$ ./install-fabric.sh

```
After successful installation, you'll see the following docker images:
![image](https://github.com/lakshya-chopra/hyperledger_docs/assets/77010972/3c867afa-ea9a-4f1d-b1b1-965b2801a41f)

And such a directory structure:
![image](https://github.com/lakshya-chopra/hyperledger_docs/assets/77010972/599c8451-499c-4a39-bfd2-4d735463a86b)

# Turn on the network and create a channel:

In your parent `hyperledger-test` directory, run the following:
```
$ cd fabric-samples/test-network
$ sudo ./network.sh up
$ sudo ./network.sh createChannel -c channel1
```
![image](https://github.com/lakshya-chopra/hyperledger_docs/assets/77010972/9898ac04-c064-4e1d-907d-091fb591634a)

![image](https://github.com/lakshya-chopra/hyperledger_docs/assets/77010972/6935127a-5456-4ea7-ad8d-39943ea1c94a)





