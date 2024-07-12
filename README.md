Does your ```apt list --upgradable```

return many packages?  You can pipe it to apt install directly with the following piping

```sh
apt list --upgradable | grep -oP '^[^/]+(?=/)' | xargs sudo apt install -y
```

you're welcome

More to come
