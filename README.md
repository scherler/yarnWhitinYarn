If you run `yarn` in a script like

```
"scripts": {
   "3": "yarn 1 && yarn 2"
}
```

you get on my system running `yarn 3`: `warning Waiting for the other yarn instance to finish (17783)` and to go on I need to kill the process by hand.

```
> uname -a
Linux mysterion 4.18.0-2-amd64 #1 SMP Debian 4.18.10-2 (2018-11-02) x86_64 GNU/Linux
> yarn -v
1.12.3

```

However I tested a couple of yarn version the problem exist in any of them. 