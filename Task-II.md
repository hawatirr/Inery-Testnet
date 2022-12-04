<b>Unlock wallet</b>

```
cline wallet unlock -n NamaWallet
```
Masukan password dari file.txt file itu didapat pada saat create wallet di task 1


<b>Generate file token.abi dan token.wasm</b>
```
cline get code inery.token -c token.wasm -a token.abi --wasm
```
<p align="center">
  <img height="auto" height="auto" src="/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FsGjdh4dhFn1XT3GtLwOJm.png&w=640&q=90 1x, /_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FsGjdh4dhFn1XT3GtLwOJm.png&w=1920&q=90 2x">
</p>

<b>Set wasm ke akun mu</b>
```
cline set code -j NamaAkun token.wasm
```

<b>Set abi ke akun mu</b>

```
cline set abi NamaAkun token.abi
```

<b>Buat Token</b>
```
cline push action inery.token create '["NamaAkun", "50000.0000 PKI" , "creating my first tokens"]' -p NamaAkun
```

<b>Deploy Token</b>
```
cline push action inery.token issue '["NamaAkun", "50000.0000 PKI", "Issuing some PKI token"]' -p NamaAkun
```

<b>Terakhir, Transfer ke 10 Akun berbeda termasuk akun inery WAJIB 1x TRANSFER KE inery WAJIB</b>
```
cline push action inery.token transfer '["NamaAkun", "TargetAkun", "1.000 PKI", "Here you go 1 PKI for free :) "]' -p NamaAkun
```

Nama Token silahkan diganti sesuka hati
