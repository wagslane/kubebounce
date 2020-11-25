# kubebounce

Command line utility to restart all of the pods in a Kubernetes namespace. Hit the project with a star if you find it useful ⭐

Supported by [Qvault](https://app.qvault.io)

## Update - There is a better way

You don't need this script. I recently found thanks to a friend a one-liner using the `kubectl` command directly.

`kubectl -n {NAMESPACE} rollout restart deploy`

I've also update the [blog post](https://qvault.io/2020/10/26/how-to-restart-all-pods-in-a-kubernetes-namespace/) on the subject.

## Install (Mac and Linux)

```
git clone https://github.com/lane-c-wagner/kubebounce
cd kubebounce
chmod +x kubebounce.sh
cp kubebounce.sh /usr/local/bin
```

## Usage

Make sure you are in the kubernetes context associated with the cluster you care about. Kubebounce depends on the [kubectl]() command.

```bash
kubebounce.sh {NAMESPACE}
```

## 💬 Contact

[![Twitter Follow](https://img.shields.io/twitter/follow/wagslane.svg?label=Follow%20Wagslane&style=social)](https://twitter.com/intent/follow?screen_name=wagslane)

Submit an issue (above in the issues tab)

## 👏 Contributing

I love help! Contribute by forking the repo and opening pull requests.

All pull requests should be submitted to the `main` branch.
