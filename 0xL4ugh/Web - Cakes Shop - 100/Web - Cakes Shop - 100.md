# Web - Cakes Shop - 100

![a.png](a.png)

When we visit the given URL we get

![b.png](b.png)

When we try to buy the **Flag Cake** we get this error

![c.png](c.png)

Try changing the requests and decreasing the Flag cake price but no luck

After looking at the Session Cookies and decoding 

![d.png](d.png)

I get the balance so after increasing the balance to say 300000 and then re-encoding the cookieas

![e.png](e.png)

and then use this cookie to get the page by using this CURL Command

```jsx
curl -i -s -k -X $'POST' \
    -H $'Host: 168.61.100.233' -H $'Content-Length: 40' \
    -b $'UserInfo=GMYDAMBQGAYA%3D%3D%3D%3D' \
    --data-binary $'flag-s=Price+%3A+1000000%24+Click+To+Buy' \
    $'http://168.61.100.233/Cakes/index.php'
```

we get the flag as 

![f.png](f.png)

## Flag - ***0xL4ugh{baSe_32_Cook!es_ArE_FuNny}***
