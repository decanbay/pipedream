# usefulbash
Does your ```apt list --upgradable```

returns many packages?  You can pipe it to apt install directly with the following command

```sh
apt list --upgradable | grep -oP '^[^/]+(?=/)' | xargs sudo apt install -y
```

you're welcome

More to come
