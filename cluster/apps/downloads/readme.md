# Torrent errors

## Ownership

Sometimes the ownership of the `downloads` folder is not correct. Connect to the NAS storage and verify.

![image](https://user-images.githubusercontent.com/37410363/193401636-97467d34-3520-4c6c-a56c-14db895a69a2.png)

If it is incorrect, use `chown` to rectify, for example

```sh
chown -R 568 downloads/
```

## File failed to allocate

Another issue I observed is "failing to allocate" space.

![image](https://user-images.githubusercontent.com/37410363/193401732-87f382d7-b6dd-47b5-bcff-543b048fb528.png)

This seems to be an issue with the following qBittorrent setting:

![image](https://user-images.githubusercontent.com/37410363/193401784-ed6aa8a1-096b-4493-bfe4-f6ef0cc9aa0e.png)

Disable this and it should go away
